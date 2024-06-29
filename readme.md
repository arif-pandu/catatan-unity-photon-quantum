### Ini contoh project pake Quantum Golf yg disediain Photon

![image](https://github.com/arif-pandu/catatan-unity-photon-quantum/assets/54800191/5a31ed7e-1031-4b43-a92d-aea374c55b43)
ini gambar contoh salah satu file .qtn sebuah object bola.

di sebuah .qtn file, ada bbrp DSL (domain-specific-language).
let's explore one by one

**input**
ini referensi linknya [sini](https://doc.photonengine.com/quantum/current/manual/input)


```
input 
{
	FPVector3 Direction;
	FP ForceBarMarkPos;
}
```

*input* ini perlu di-subscribe sama file di Unity
```
private void OnEnable()
{
  QuantumCallback.Subscribe(this, (CallbackPollInput callback) => PollInput(callback));
}
```


