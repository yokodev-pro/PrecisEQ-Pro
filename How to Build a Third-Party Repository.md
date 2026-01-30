# How to Build a Third-Party Repository
## Calibration Files
Currently, the client only supports FIR, with the following format requirements:
- The sampling format must use **32 bits IEEE Stereo** (.wav). Ensure minimum phase is used, and use the same calibration to generate four sample-rate versions: **44, 48, 96, and 192**.
- The frequency response after calibration must be a horizontally flat curve; the target curve actually used will be restored on the client via EQ.
- All calibration files must be set with a **-12 dB** pre-gain.
- For measurement artificial ears, **B&K 4195** (in-ear) and **GRAS RA0045+KB0060** (over-ear) are recommended, or compensate to an approximate equivalent.
## Deployment Files
Reference directory file structure:
```text
.
├── headphone_list.json           # Headphone list description file
├── repo_info.json                # Repository information description file
├── inear_1_44.wav                # Headphone calibration file (sample rate 44.1kHz)
├── inear_1_48.wav                # Headphone calibration file (sample rate 48kHz)
├── inear_1_96.wav                # Headphone calibration file (sample rate 96kHz)
├── inear_1_192.wav               # Headphone calibration file (sample rate 192kHz)
├── hpopen_2_44.wav               # Headphone calibration file (sample rate 44.1kHz)
├── hpopen_2_48.wav               # Headphone calibration file (sample rate 48kHz)
├── hpopen_2_96.wav               # Headphone calibration file (sample rate 96kHz)
├── hpopen_2_192.wav              # Headphone calibration file (sample rate 1921kHz)
├── hpclose_3_44.wav              # Headphone calibration file (sample rate 44.1kHz)
├── hpclose_3_48.wav              # Headphone calibration file (sample rate 48kHz)
├── hpclose_3_96.wav              # Headphone calibration file (sample rate 96kHz)
├── hpclose_3_192.wav             # Headphone calibration file (sample rate 192kHz)
……
```
- The naming format for headphone calibration files is `id_version_samplerate`.
- Each `id` must provide four sample rates: 44.1, 48, 96, and 192.
- All files (`headphone_list.json`, `repo_info.json`, and the headphone calibration files) are placed in the same directory. The URL pointing to that directory is the repository address.

Reference content for `headphone_list.json`:
```json
[
  {
    "id": "inear",
    "type": 0,
    "brandName": [
      "Brand",
      "品牌名"
    ],
    "modelName": [
      "Model Name",
      "型号名"
    ],
    "version": 1,
    "noDspOffsetDb": 0
  },
  {
    "id": "hpopen",
    "type": 1,
    "brandName": [
      "Brand"
    ],
    "modelName": [
      "Model Name",
      "型号名"
    ],
    "version": 2,
    "noDspOffsetDb": 1.5
  },
  {
    "id": "hpclose",
    "type": 2,
    "brandName": [
      "Brand",
      "品牌名"
    ],
    "modelName": [
      "Model Name"
    ],
    "version": 3,
    "noDspOffsetDb": -1
  }
]
```
The client generates the headphone list based on `headphone_list.json`, and combines `id` and `version` to index the calibration files.  
- `id`: The unique identifier of the headphone calibration file within this repository; it must not be duplicated.  
- `type`: The headphone type, specified as one of the following three: `0` for in-ear, `1` for open-back over-ear, and `2` for closed-back over-ear.  
- `brandName`: Brand name; the second line is the Chinese name. When the client uses Chinese localization, it will display the second line rather than the first.  
- `modelName`: Model name; the second line is the Chinese name. When the client uses Chinese localization, it will display the second line rather than the first. If a model has multiple sound modes—for example, If a model has multiple sound modes—for example, when the ANC is on/off—each mode should be calibrated separately, listed individually with a different id, and distinguished within this field.  
- `version`: A positive non-zero integer. It must be kept in sync with the `version` field in the file name. Headphones uploaded for the first time should be set to `1`. When uploading new calibration files, this value must be monotonically increasing.  
- `noDspOffsetDb`: In dB. Because the perceived loudness after calibration for some headphones may differ significantly from before calibration, this value can be used to increase/decrease the pre-calibration volume.  

Reference content for `repo_info.json`:
```json
{
  "name": "Repository name",
  "maintainer": "Repository maintainer",
  "description": "Explain the usage precautions of this repository to users."
}
```
The client displays repository information based on `repo_info.json`.
