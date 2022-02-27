# README #

Este README descreve o funcionamento e dependências do projeto de realidade aumentada criado utilizando Unity3d, Vuforia e uma WebApi.

## Das versões de softwares 

1.	Unity3D 2019.2.17f1
2.	Vuforia 9.1.7
3.	SimpleJSON, versão não definida
4.	Android Studio 4.0.1 for Windows 64-bit 
5.	SDK Java "1.8.0_111" 
6.	SDK Android 28 
7.  Dropbox.Api.dll @latest na pasta plugins (se atualizado deve ser inserido na pasta MANUALMENTE)

## Funcionamento dos scripts

- Fluxo normal:
	-	TargetManager é acionado a partir de um gameobject de mesmo nome
	-	A dependência do Script é NetworkService  e faz uma web request para um endpoint
	-	Os dados são carregados e retornados 
	-	A class EventHandler responsável pela comunicação com o Vuforia é inserido no gameobject (veja como: https://www.youtube.com/watch?v=9XikHnTiukk&list=PLX2vGYjWbI0Thl0pOCbKWrbbiw7RWiRG7).
	-	A class TrackingComponentManager é chamada para criar conteúdo em real time (resource types e media)
	-	Cada resource class tem métodos próprios definidos nos components

## Recursos de Apoio

- https://www.udemy.com/course/the-ultimate-guide-to-real-world-applications-with-unity/learn/lecture/11600536?start=450#overview
- https://www.youtube.com/watch?v=MtiUx_szKbI
- https://www.youtube.com/watch?v=ElmzIq6stNI&t=12s
- https://docs.unity3d.com/Packages/com.unity.ugui@1.0/manual/index.html
