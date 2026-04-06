# muhammedfurkanakarsu
homework
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class CameraController : MonoBehaviour
{
 public GameObject player;

 private Vector3 offset;

 void Start()
    {
        offset = transform.position - player.transform.position; 
    }

 void LateUpdate()
    {
        transform.position = player.transform.position + offset;  
    }
}

bu kodda 
UnassignedReferenceException: The variable player of CameraController has not been assigned.
You probably need to assign the player variable of the CameraController script in the inspector.
UnityEngine.Object+MarshalledUnityObject.TryThrowEditorNullExceptionObject (UnityEngine.Object unityObj, System.String parameterName) (at /Users/bokken/build/output/unity/unity/Runtime/Export/Scripting/UnityEngineObject.bindings.cs:1072)
UnityEngine.Bindings.ThrowHelper.ThrowNullReferenceException (System.Object obj) (at /Users/bokken/build/output/unity/unity/Runtime/Export/Scripting/BindingsHelpers.cs:61)
UnityEngine.GameObject.get_transform () (at <1152e6f144b34848838e1c9abaceb7cf>:0)
CameraController.LateUpdate () (at Assets/Scripts/CameraController.cs:18)

böyle bir hata oluyorum sorun nedir?

Bu hatanın çözümünü yapay zekaya sorarak öğrendim aslında basit bir işlem gerekiyormuş ama başlangıç için baya zorlandım.