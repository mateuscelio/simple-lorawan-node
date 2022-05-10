# Simple LoRaWAN node

## Setup

1. run `pio run`

2. Deps will be downloaded and builded but during `MCCI LoRaWAN LMIC library` building an
   error will be raised:

   ```
    25 | # error You can define at most one of CFG_... variables
   ```

   open the file `.pio/libdeps/bluepill_f103c8/MCCI LoRaWAN LMIC library/project_config/lmic_project_config.h` and comment any defined `CFG_*`

3. Build again using `pio run`
