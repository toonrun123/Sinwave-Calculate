# Sinwave-Calculate

## SIN CALCULATE:
### x = wave value
### a = height wave
### h = wave position
### b = wave noise
### k = wave Position Y

## Example
```lua
local sine:ModuleScript = require(YOUR_PATH_MODULE)
local sinwave = sine:new(0,10,0,5,3.5) --[[x,a,h,b,k]]

for X = 1,360 do
	sinwave.x = X
	local Y = sinwave:wave()
	local Part:Part = Instance.new("Part",workspace)
	Part.Position = Vector3.new(0,Y,X)
	Part.Anchored = true
end
```
