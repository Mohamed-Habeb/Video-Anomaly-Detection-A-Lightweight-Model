# Video-Anomaly-Detection-A-Lightweight-Model

# UCSD Test Video 2 Anomaly Score
<p>
<img src="https://github.com/Mohamed-Habeb/Video-Anomaly-Detection-A-Lightweight-Model/blob/main/UCSD_Test02.gif" width="300" height="400" />

<img src="https://github.com/Mohamed-Habeb/Video-Anomaly-Detection-A-Lightweight-Model/blob/main/UCSD_test_video02.gif" width="300" height="400" />
</p>


# CUHK Avenue Test Video 5 Anomaly Score

<p>
<img src="https://github.com/Mohamed-Habeb/Video-Anomaly-Detection-A-Lightweight-Model/blob/main/CUHK_Test05.gif" width="300" height="400" />

<img src="https://github.com/Mohamed-Habeb/Video-Anomaly-Detection-A-Lightweight-Model/blob/main/CUHK_Test_Video05.gif" width="300" height="400" />
</p>

<p>
let imgs = [
  "https://github.com/Mohamed-Habeb/Video-Anomaly-Detection-A-Lightweight-Model/blob/main/UCSD_Test02.gif",
  "https://github.com/Mohamed-Habeb/Video-Anomaly-Detection-A-Lightweight-Model/blob/main/UCSD_test_video02.gif",
] //all files there

preload = async(images) => {

  let load = imgs.map(async a => {
    let img = new Image()
    img.src = a
    return await new Promise(res => {
      img.onload = () => res(img)
    })


  })


  const results = await Promise.all(load)

  console.log(results)
}

preload(imgs)
</p>
