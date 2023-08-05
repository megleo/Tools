# Synergy

I have 3 computers : Ubuntu 18.04(server), jetson orin nano (8G client), windows 10 (lenovo L14 )

On server

1. mv.synergy.conf to ${Home}/
2. ```
   synergys -f --no-tray --debug DEBUG2 --name ubuntu3060 --address :24800
   ```

## On client (nano)

1. ```shell

   synergy-core client --no-daemon --name nano 10.0.73.31:24800
   ```

## On client(windows)

Just click the windos is ok.



# Complier

For Jetson orin nano, which CPU architecture is arm64, that need COMPILER.

just execute the jeston_orin_nano_synergy_compiler_script.sh

This shell script is got from github, which I forget the repo name.

.
├── jetson_orin_nano_sysnergy_compiler_script.sh
└── README.md