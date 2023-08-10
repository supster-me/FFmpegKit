# FFmpegKit for SUPSTER_FLUTTER

Сборка на основе пакета [FFmpegKit](https://github.com/arthenica/ffmpeg-kit)

### 1. Features

- Includes both `FFmpeg` and `FFprobe`
- Supports
    - `Android`, `iOS`
    - FFmpeg `v5.1.2`
    - `arm-v7a`, `arm-v7a-neon`, `arm64-v8a`, `x86` and `x86_64` architectures on Android
    - `Android API Level 24` or later
      architectures on iOS
    - `iOS SDK 12.1` or later
      - `iOS SDK 10` on LTS releases
    - `arm64` and `x86_64` architectures on macOS
    - `macOS SDK 10.15` or later
      - `macOS SDK 10.12` on LTS releases
    - Android config:
      - --enable-shared \
        --disable-static \
        --disable-doc \
        --disable-programs \
        --disable-postproc \
        --disable-network \
        --disable-debug \
        --disable-asm \
        --enable-small \
        --disable-everything \
        --enable-encoder=opus,aac,libopus \
        --enable-decoder=opus,aac,libopus \
        --enable-muxer=opus,ogg,oga \
        --enable-demuxer=mov \
        --enable-protocol=file \
        --enable-filter=aformat,anull,atrim,format,hflip,null,transpose,trim,vflip,aresample \
        --enable-libopus
