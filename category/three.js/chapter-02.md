---
layout: post
title: chapter02 - Three.js 구조 이해와 간단한 scene 만들기
tags: [three.js, javascript, front-end, js, 3D, WebGL]
comments: true
---

[Three.js 참조 (Click)](https://threejsfundamentals.org/threejs/lessons/kr/threejs-fundamentals.html)

# Three.js의 구조
Three.js로 구현하기 위해서는 기본적으로 아래의 4가지가 필요하다. scene, camera, renderer, HTML  
* HTML : Three.js를 표현할 공간
* scene : Scene 또는 다수의 Mash, Light, Group, Object3D, camera 로 이루어진 씬 그래프보다 위에있는 최상위 노드로서 배경색, 안개 등의 요소를 포함한다.
* renderer : Three.js의 핵심 개체로서, renderer는 scene과 camera 객체를 넘겨 받아 카메라의 절두체 안 3D 씬의 일부를 평면 이미지로 렌더링한다.
* camera : 화면에 어떤 것이 렌더링될 것인지 결정하는 것이다 즉, 장면을 보여주는 역할이다.

이 외
* Mash : 간단하게는 하나의 객체이다. 자세하게는 Material로 하나의 Geometry를 그리는 객체이다. Material와 Geometry는 재사용이 가능하다. 파란색 정육면체 2개를 그린다고 가정했을 때, 두 정육면체는 위치가 다르니 2개의 Mash가 필요하다. 그리고 정점 데이터를 가진 한 개의 Geometry와 채색을 위한 하나의 Material이 필요하다. 이때 각 Mash는 객체를 복사할 필요 없이, 같은 Geometry 그리고 Material을 참조할 수 있습니다.
* Geometry : 기하학 객체의 정점 데이터이다. 구, 사각형, 정육면체, 면, 사람, 자동차, 건물, 해 등 
* Material : 위의 기하학 객체를 그리는 데 필요한 **표면속성** 이다. 색, 밝기 등을 지정할 수 있다. 여러개의 Texture를 사용할 수 있다.
* Texture : 이미지나 파일에서 로드한 이미지, canvas로 생성한 이미지, 다른 scene 객체에서 렌더링한 결과물에 해당한다.
* Light : 여러 종류의 광원에 해당한다.

