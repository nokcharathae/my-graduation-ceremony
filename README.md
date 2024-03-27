# 나의 졸업식

You can [try it out here](https://nokcharathae.github.io/my-graduation-ceremony/).

 
이 웹은 저의 메타버스 졸업식에 참석하기 위한 페이지입니다. 데이터는 이미지로부터 3차원 표현을 가능케 한 <a href="https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/" target="_blank">3D Gaussian Splatting for Real-Time Radiance Field Rendering</a>으로부터 학습시켜 얻었습니다. 제 졸업식에 어서오세요!

## Reference 
코드는 아래를 참고하여 작성하였습니다.
- <a href="https://github.com/antimatter15/splat" target="_blank">animatter15/splat</a>
- <a href="https://github.com/Anttwo/SuGaR" target="_blank">Anttwo/SuGaR</a>

## To do
- 컨트롤러 수정(메타버스처럼 움직일 수 있도록)
- variation 추가
- decals(졸업을 축하해 이모티콘) 기능 추가
- 댓글 기능 추가


## controls

movement (arrow keys)

- left/right arrow keys to strafe side to side
- up/down arrow keys to move forward/back
- `space` to jump

camera angle (wasd)

- `a`/`d` to turn camera left/right
- `w`/`s` to tilt camera up/down
- `q`/`e` to roll camera counterclockwise/clockwise
- `i`/`k` and `j`/`l` to orbit

trackpad
- scroll up/down to orbit down
- scroll left/right to orbit left/right
- pinch to move forward/back
- ctrl key + scroll up/down to move forward/back
- shift + scroll up/down to move up/down
- shift + scroll left/right to strafe side to side

mouse
- click and drag to orbit
- right click (or ctrl/cmd key) and drag up/down to move forward/back
- right click (or ctrl/cmd key) and drag left/right to strafe side to side

touch (mobile)
- one finger to orbit
- two finger pinch to move forward/back
- two finger rotate to rotate camera clockwise/counterclockwise
- two finger pan to move side-to-side and up-down

other
- press 0-9 to switch to one of the pre-loaded camera views
- press '-' or '+'key to cycle loaded cameras
- press `p` to resume default animation
- drag and drop .ply file to convert to .splat
- drag and drop cameras.json to load cameras

## other features

- press `v` to save the current view coordinates to the url
- open custom `.splat` files by adding a `url` param to a CORS-enabled URL
- drag and drop a `.ply` file which has been processed with the 3d gaussian splatting software onto the page and it will automatically convert the file to the `.splat` format




## acknowledgements

Thanks to Otavio Good for discussions on different approaches for [order independent transparency](https://en.wikipedia.org/wiki/Order-independent_transparency), Mikola Lysenko for [regl](http://regl.party/) and also for helpful advice about webgl and webgpu, Ethan Weber for discussions about how NeRFs work and letting me know that sorting is hard, Gray Crawford for identifying issues with color rendering and camera controls, Anna Brewer for help with implementing animations, and GPT-4 for writing all the WebGL boilerplate. 
