[@zeldafan0225/ai_horde](../README.md) / [Exports](../modules.md) / ModelGenerationInputStable

# Interface: ModelGenerationInputStable

## Table of contents

### Properties

- [cfg\_scale](ModelGenerationInputStable.md#cfg_scale)
- [clip\_skip](ModelGenerationInputStable.md#clip_skip)
- [control\_type](ModelGenerationInputStable.md#control_type)
- [denoising\_strength](ModelGenerationInputStable.md#denoising_strength)
- [facefixer\_strength](ModelGenerationInputStable.md#facefixer_strength)
- [height](ModelGenerationInputStable.md#height)
- [hires\_fix](ModelGenerationInputStable.md#hires_fix)
- [image\_is\_control](ModelGenerationInputStable.md#image_is_control)
- [karras](ModelGenerationInputStable.md#karras)
- [n](ModelGenerationInputStable.md#n)
- [post\_processing](ModelGenerationInputStable.md#post_processing)
- [return\_control\_map](ModelGenerationInputStable.md#return_control_map)
- [sampler\_name](ModelGenerationInputStable.md#sampler_name)
- [seed](ModelGenerationInputStable.md#seed)
- [seed\_variation](ModelGenerationInputStable.md#seed_variation)
- [steps](ModelGenerationInputStable.md#steps)
- [tiling](ModelGenerationInputStable.md#tiling)
- [toggles](ModelGenerationInputStable.md#toggles)
- [width](ModelGenerationInputStable.md#width)

## Properties

### cfg\_scale

• `Optional` **cfg\_scale**: `number`

its how much the AI listens to your prompt, essentially.

**`Default`**

5

**`Minimum`**

-40

**`Maximum`**

30

Multiple of 0.5

#### Defined in

[index.ts:1923](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1923)

___

### clip\_skip

• `Optional` **clip\_skip**: `number`

The number of CLIP language processor layers to skip

**`Minimum`**

1

**`Maximum`**

12

#### Defined in

[index.ts:1977](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1977)

___

### control\_type

• `Optional` **control\_type**: `canny` \| `hed` \| `depth` \| `normal` \| `openpose` \| `seg` \| `scribble` \| `fakescribbles` \| `hough`

#### Defined in

[index.ts:1978](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1978)

___

### denoising\_strength

• `Optional` **denoising\_strength**: `number`

The strength of denoising

**`Minimum`**

0

**`Maximum`**

1

Multiple of 0.01

#### Defined in

[index.ts:1931](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1931)

___

### facefixer\_strength

• `Optional` **facefixer\_strength**: `number`

**`Example`**

```ts
0.75
```

**`Minimum`**

0

**`Maximum`**

1

#### Defined in

[index.ts:1994](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1994)

___

### height

• `Optional` **height**: `number`

The height of the image to generate

**`Default`**

512

**`Minimum`**

64

**`Maximum`**

3072

Multiple of 64

#### Defined in

[index.ts:1942](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1942)

___

### hires\_fix

• `Optional` **hires\_fix**: `boolean`

Set to True to process the image at base resolution before upscaling and re-processing

**`Default`**

false

#### Defined in

[index.ts:1971](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1971)

___

### image\_is\_control

• `Optional` **image\_is\_control**: `boolean`

Set to True if the image submitted is a pre-generated control map for ControlNet use

**`Default`**

false

#### Defined in

[index.ts:1983](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1983)

___

### karras

• `Optional` **karras**: `boolean`

Set to True to enable karras noise scheduling tweaks

#### Defined in

[index.ts:1959](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1959)

___

### n

• `Optional` **n**: `number`

The amount of images to generate

**`Minimum`**

1

**`Maximum`**

20

#### Defined in

[index.ts:2006](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L2006)

___

### post\_processing

• `Optional` **post\_processing**: `ModelGenerationInputPostProcessingTypes`[]

The list of post-processors to apply to the image, in the order to be applied

#### Defined in

[index.ts:1961](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1961)

___

### return\_control\_map

• `Optional` **return\_control\_map**: `boolean`

Set to True if you want the ControlNet map returned instead of a generated image

**`Default`**

false

#### Defined in

[index.ts:1988](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1988)

___

### sampler\_name

• `Optional` **sampler\_name**: `k_lms` \| `k_heun` \| `k_euler` \| `k_dpm_2` \| `k_dpm_2_a` \| `DDIM` \| `PLMS` \| `k_dpm_fast` \| `k_dpm_adaptive` \| `k_dpmpp_2s_a` \| `k_dpmpp_2m` \| `dpmsolver`

**`Default`**

k_euler

#### Defined in

[index.ts:1910](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1910)

___

### seed

• `Optional` **seed**: `string`

The seed to use to generete this request.

#### Defined in

[index.ts:1933](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1933)

___

### seed\_variation

• `Optional` **seed\_variation**: `number`

If passed with multiple n, the provided seed will be incremented every time by this value

**`Minimum`**

1

**`Maximum`**

1000

#### Defined in

[index.ts:1957](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1957)

___

### steps

• `Optional` **steps**: `number`

**`Default`**

30

**`Minimum`**

1

**`Maximum`**

500

#### Defined in

[index.ts:2000](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L2000)

___

### tiling

• `Optional` **tiling**: `boolean`

Set to True to create images that stitch together seamlessly

**`Default`**

false

#### Defined in

[index.ts:1966](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1966)

___

### toggles

• `Optional` **toggles**: `number`[]

Special Toggles used in the SD Webui. To be documented.

#### Defined in

[index.ts:1914](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1914)

___

### width

• `Optional` **width**: `number`

The width of the image to generate

**`Default`**

512

**`Minimum`**

64

**`Maximum`**

3072

Multiple of 64

#### Defined in

[index.ts:1951](https://github.com/ZeldaFan0225/ai_horde/blob/79ac96e/index.ts#L1951)
