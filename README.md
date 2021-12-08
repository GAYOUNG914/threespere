# Three.js sphere 생성
webpack 환경에서 Three.js 라이브러리와 자바스크립트를 사용하여 인터랙티브한 구를 구현해보았습니다.


## Link
* https://gayoung914.github.io/threespere/

## Tool
* HTML5
* CSS3
* Three.js

## Skill
* dat.gui 사용
  - **dat.gui debug tool**<br>
    👉 dat.gui를 사용함으로써 직관적, 시각적인 debug tool을 제공 받을 수 있습니다.
```
  const light1 = gui.addFolder('Light 1') //.addFolder() 메소드로 폴더를 만들수도있다.

  light1.add(pointLight2.position, 'y').min(-3).max(3).step(0.01)
  //y 포지션만 컨트롤 하고싶다, 근데 최소 3 최대 3값으로, 0.01씩 움직이는거 보여줘
  light1.add(pointLight2.position, 'x').min(-6).max(6).step(0.01)
  light1.add(pointLight2.position, 'z').min(-3).max(3).step(0.01)
  light1.add(pointLight2, 'intensity').min(0).max(10).step(0.01)
  
  //위의 gui를 사용하여 원하는 값을 아래와 같이 넣어주면 된다.
  
  const pointLight2 = new THREE.PointLight(0xeeeeee, 0.1)
  // pointLight.position.x = 2
  // pointLight.position.y = 3
  // pointLight.position.z = 4 
  pointLight2.position.set(-1.73,1.6,-1.84) //x,y,z 한 번에 쓸 수 있음
  pointLight2.intensity = 6

  scene.add(pointLight2)
  
```

(내용 추가 및 수정 중입니다.)

## License
개인 포트폴리오를 위해 만들어진 사이트입니다.

