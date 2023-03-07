# onnx_stable_diffusion_controlnet
WIP: Get Stable DIffusion Controlnet running with DirectML via ONNX
<br>The original conversion script is frome here: https://github.com/Amblyopius/Stable-Diffusion-ONNX-FP16
<br>I couldn't figure out how to pass a tuple of tensors as an input with Onnxruntime, so I just modified UNet2DConditionModel and renamed it UNet2DConditionModel_Cnet so that instead of a tuple of 12 tensors, it's 12 separate tensors passed as individual arguments.
