# Regularization class images for Dreambooth Training - SD 2.1
I've created a set of training images for StableDiffusion 2.1, as I couldnt find any classification images in `768x768`.

Do note, that this is by no means a solved problem, and I am just testing out different class image sets and prompt combinations.
> 
## Usage
Refer to the table below, and based on which set of images you choose, select the prompt you want accordingly. Replace `<instance>` with the name of your instance.

|Folder		|Class Prompt	|Negative Prompt	|Instance Prompt to use	|Remarks	|
|------		|---			|---				|---					|---		|
|[`person`](/person/)	|`person`		|None				|`<instance> person`	|Your basic, gender-neutral class images. Mileage may vary (training this on my face, I've gotten very quite inaccurate results frequently)|
|[`photo of a person`](/photo%20of%20a%20person/)|`person`|`ugly, deformed`|`<instance> person`	|Better results for photographic outputs, but feels like it doesnt retain faces that well, and different art styles are comparatively more difficult to achieve.

<details><summary>Generation details</summary>
<p>

## Generation details for class images

|Class		            |Sampler	|Steps	|CFG Scale	|
|------		            |---		|---	|---		|
|`person`	            |`DDIM`		|`40`	|`7`		|
|`photo of a person`	|`DDIM`		|`40`	|`7`		|

</p>
</details>