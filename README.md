# OCV-face68-StaticStore
OpenCV Face68 StaticStore Example. Unity C# Script.

## static class

```
namespace DMT
{
    public static class StaticStore
    {

    }
}
```

## getter/setter for NoseNDC, Mouth, PointMovement 2DVector

```
public static Vector2 NoseNDC { get; set; }
public static double MouthOpen { get; set; }
public static float leftRightFace { get; set; }
public static float upDownFace { get; set; }
```

## getter/setter for BoundingBox (NDC)

```
private static UnityEngine.Rect _boundingBoxNDC = Rect.zero;

public static UnityEngine.Rect myBoundingBoxNDC // main BoundingBoxes
{
    get { return _boundingBoxNDC; }
    set
    {
        UnityEngine.Rect gotData = value;
        _boundingBoxNDC = gotData;
    }
}
```
