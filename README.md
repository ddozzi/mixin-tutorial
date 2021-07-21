# Mixin Tutorial - INTELLJI
I haven't seen any decent mixin tutorials, so here's one.

## Topics

- Setting up your first mixin project
- Creating your first mixin

## Setup

Create a new folder where ever you want your client to be. 
![Example Client](https://user-images.githubusercontent.com/69029714/126436967-facffba9-a63e-4c8a-9cd6-3837cfe62a44.png)

Open up IntelliJ. Then click `New Project > Gradle > Next`. Set the `Location` to the folder you just created
![EC INTELLIJ](https://user-images.githubusercontent.com/69029714/126437646-557d291c-851d-424f-87ca-062d79c3461b.png)



Copy and paste the ![build.gradle](https://github.com/ddozzi/Mixin-Tutorial/blob/main/build.gradle) into your `build.gradle`.
![EC INTELLIJ 2](https://user-images.githubusercontent.com/69029714/126437757-62a7b876-785b-41d4-928d-04e841f3685a.png)

Then click the "Load Gradle Changes" Button on the top right.
![refresh button](https://user-images.githubusercontent.com/69029714/126437993-ae1b7358-0335-4651-8cb5-1fdc0d716383.png)

You might be noticing an error popping up in the bottom half, that's totally normal. It's because forgegradle doesn't support newer versions of gradle.

![Screen Shot 2021-07-21 at 1 52 50 AM](https://user-images.githubusercontent.com/69029714/126438050-42e89148-3242-44b7-8c84-c977efb74350.png)

To fix this, go to `gradle > wrapper > gradle-wrapper.properties` then replace whatever version is currently there, with 4.7


https://user-images.githubusercontent.com/69029714/126439227-39686823-fe4f-49fe-bb84-0a86235286c0.mov


Now for the lengthy part. Replace all the "example" strings with your client name. Also replace the "net" packages with whatever fits you. An example is shown below. **This MUST be done for all instances. DO NOT CHANGE ANY OF THE "mixin" OR "mixins" strings **

Once you are done, click the gradle button on the far right. Then click `Tasks > forgegradle > setupDecompWorkspace`. This will take some time.
![Screen Shot 2021-07-21 at 2 09 49 AM](https://user-images.githubusercontent.com/69029714/126439713-851590a2-9733-4ee3-8645-89234d3528e6.png)

Once that process is finished, click `Tasks > forgegradle > genIntellijRuns`
![Screen Shot 2021-07-21 at 2 10 32 AM](https://user-images.githubusercontent.com/69029714/126439793-ecbd06b3-632c-44e3-b28d-a43684b6db8f.png)

Click the button at the top then click `Minecraft Client` An example is shown below.

https://user-images.githubusercontent.com/69029714/126440150-9632bb22-8278-467e-ad86-425d15ffa2ec.mov

Click the same button again, then click `Edit Configurations`



## Tweaker

Create a new package in `src/main/java
