# Summary: 
- Expo video player issue (Android) with public drive link.
- I tried with 3 type of link to play video in expo video, but only 2 was working.

## How to run:
- run `npm install`
- run `npm start`
- to test different types of video select from below table and add in `App.tsx` file

### Expected behavior:
- All 3 type of link should play video in android and ios both


### Actual Behavior:
- Only .m3u8 and direct link is working with both android and ios.
- For drive link it's only working with IOS, but in android it give blank screen and nothing else. No error either.
- Here is the full details table.

| Android | IOS | Urls |
| --------------------- | --------------------- | --------------------- |
| :x: | :heavy_check_mark: | https://drive.google.com/uc?export=download&id=1eQE1Cq9UcYQych-c3xcKeRNaE5yMvy85 |
| :heavy_check_mark: | :heavy_check_mark: | https://devstreaming-cdn.apple.com/videos/streaming/examples/img_bipbop_adv_example_fmp4/master.m3u8 |
| :heavy_check_mark: | :heavy_check_mark: | https://d23dyxeqlo5psv.cloudfront.net/big_buck_bunny.mp4 |


### Tested Device and environment.
- Android emulator (Pixel 8 pro - Android 12)
- Physical devices (Nokia 6X - Android 10) / (IPhone 14 plus)
- Expo snack [Open snack](https://snack.expo.dev/@deviser/video)

### Note:

- It was working with expo sdk: "~47.0.12"
- once upgraded to sdk 50 it stopped working.