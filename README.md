# STM32-custom-HID
STM32 custom HID game controller

Bu projede STM32 custom HID game controller yapısı üzerinden nasıl descriptor hazırlanır, nasıl STM HAL kütüphaneleri ile USB üzerinden veri buton ve joystick verisi gönderileceğini anlatacağım.

Ben bu projemde STM32F407G DISCOVERY kart kullandım. Ayırca ilerleyen günlerde STM32F103C8T6 (blue pill) ile de bu prjeyi tekrarlamak istiyorum. Onun kodlarını ve nasıl yaptığımı da anlatacağım.

İlk olarak usb descriptor'dan ve nasıl hazırlanacağından bahsedeyim:
  USB descriptor, usb üzerinden bir aygıt bağladığımızda işletim sistemi tarafından bağlanan cihazın ne olduğunu (mouse, game controller, mass storage device, vb), kaç bit veri göndereceğini, eğer varsa hangi butonlara sahip olduğunu, vb bilgilerin barındırıldığı bilgidir. USB descriptor tek sefer gönderilir.
  Hazırlanması için USB'nin sitesinde bulunan USB Descriptor Tool'u kullanacağız.
    Link: https://www.usb.org/document-library/hid-descriptor-tool

![image](https://user-images.githubusercontent.com/89520252/186914383-8a184ba7-efb7-4e18-9034-4f28f9ebd0b6.png)

  Descriptor oluştururken öncelikle bu cihazın hangi ürün ailesi ait olduğundan bahsetmemiz gerekecektir. Bunun için "usage_page" eklememiz gerekiyor...
  

  
  Devam edecek.
  
