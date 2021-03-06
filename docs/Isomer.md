## Module Isomer

#### `ISOMER`

``` purescript
data ISOMER :: !
```

#### `IsomerInstance`

``` purescript
data IsomerInstance :: *
```

#### `IsomerColor`

``` purescript
data IsomerColor :: *
```

#### `getIsomerInstance`

``` purescript
getIsomerInstance :: forall eff. String -> Eff (isomer :: ISOMER | eff) IsomerInstance
```

(Install and) return the Isomer instance on the canvas with the given id

#### `renderBlock`

``` purescript
renderBlock :: forall eff. IsomerInstance -> Number -> Number -> Number -> Number -> Number -> Number -> IsomerColor -> Eff (isomer :: ISOMER | eff) Unit
```

Render a colored block of size dx, dy, dz at position x, y, z

#### `renderCube`

``` purescript
renderCube :: forall eff. IsomerInstance -> Number -> Number -> Number -> IsomerColor -> Eff (isomer :: ISOMER | eff) Unit
```

Render a single colored cube at the given position

#### `clearCanvas`

``` purescript
clearCanvas :: forall eff. IsomerInstance -> Eff (isomer :: ISOMER | eff) Unit
```

Clear the whole canvas that belongs to the Isomer instance

#### `setIsomerConfig`

``` purescript
setIsomerConfig :: forall eff. IsomerInstance -> Number -> Number -> Number -> Eff (isomer :: ISOMER | eff) Unit
```

Set Isomer scale factor and origin (X and Y)

#### `colorFromRGB`

``` purescript
colorFromRGB :: Int -> Int -> Int -> IsomerColor
```

Create Isomer.Color object from its RGB representation


