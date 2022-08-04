# Fetch header files from
- https://github.com/MarlinFirmware/Configurations/tree/bugfix-2.1.x/config/examples/Creality/Ender-3%20Pro/BigTreeTech%20SKR%20Mini%20E3%202.0

# platformio.ini
- `default_envs = STM32F103RC_btt_512K`
# Configuration.h
- uncomment 
    - `#define BLTOUCH`
    - `#define USE_PROBE_FOR_Z_HOMING`
    - `#define Z_SAFE_HOMING`
    - `#define AUTO_BED_LEVELING_BILINEAR`
- comment
    - `//#define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN`
    - `//#define MIN_SOFTWARE_ENDSTOP_Z` 
    - `//#define MESH_BED_LEVELING`
- set
    - `#define Z_MIN_PROBE_PIN PC14`
    - `#define NOZZLE_TO_PROBE_OFFSET { -45, -7, 0 }`

# Configuration_adv.h
- uncomment
    - `#define BLTOUCH_DELAY 500`
    - `#define BLTOUCH_FORCE_SW_MODE`
    - `#define PROBE_OFFSET_WIZARD`
    - `#define PROBE_OFFSET_WIZARD_START_Z -4.0`
    - `#define BABYSTEP_DISPLAY_TOTAL`
    - `#define BABYSTEP_ZPROBE_OFFSET`
- comment
- set