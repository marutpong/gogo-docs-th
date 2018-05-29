# 7.4 การควบคุมมอเตอร์เซอร์โว

การควบคุมมอเตอร์เซอร์โวมักจะหมายถึงการตั้งตำแหน่งมอเตอร์ตามต้องการ คำสั่งการดำเนินการนี้ ในภาษาโลโกคือ “**seth**” ซึ่งย่อมาจาก “set heading” ใน Tinker ใช้บล็อก “Set servo heading” พิจารณาดังตัวอย่างต่อไปนี้

{% tabs %}
{% tab title="Logo" %}
```text
to servo_control
    a, seth 10
    wait 10
    seth 40
end
```
{% endtab %}

{% tab title="Tinker" %}
![](https://lh4.googleusercontent.com/PkmsY5-cdQdVwbAopSlrqHpR7Jv5qdOaXAQBVsUFYRu2SJNSxbpRt7mhYs3Hy20a6yt_RV5rIIBncz3jdMnbty0fHZ75TYTb4vwGAmCdNQRIMrX3-MDVclbIgTv-_xJMFzDH39Qe)
{% endtab %}
{% endtabs %}

จากตัวอย่างข้างต้น มอเตอร์เซอร์โวจะเชื่อมต่อกับพอร์ตเซอร์โว A และตั้งค่าตำแหน่งเซอร์โวเป็น 10 รอ 1 วินาทีแล้วหมุนเซอร์โวไปที่ตำแหน่ง 40

ตำแหน่งที่ 10 และตำแหน่งที่ 40

![](https://lh5.googleusercontent.com/xtZp4ZZl4JNFAgu8kyWSmIFpz0SxSFi2ntoOE3QUd8pL_MhZELgxHFgT0YgFS0w38-FUdsYMNWRx0kAqkeN9XruZ7gXuftvatO05IDgA-FmVsGJd-sIU-IKQD3q_PyMbPxiQhq9k)

## ตำแหน่งทิศทางของมอเตอร์เซอร์โว {#servo-motor-heading-position}

ตำแหน่งที่ 10 หรือ 40 ในตัวอย่างข้างต้น เป็นหมายเลขตำแหน่งในโกโกบอร์ด ซึ่งไม่มีหน่วยมาตรฐานใดๆ ดังนั้นคุณต้องกำหนดตัวเลขที่ใช้เพื่อให้มอเตอร์ชี้ไปยังทิศทางที่ต้องการ ทำได้ง่ายโดยใช้ **GoGo Widget** ตามที่อธิบายไว้ก่อนหน้านี้

{% hint style="warning" %}
ห้ามใช้ตำแหน่งที่เกินขอบเขตของเซอร์โว เนื่องจากเซอร์โวไม่สามารถหมุนเป็นวงกลมเต็มวง มิฉะนั้นจะทำลายฟันเฟืองภายในเซอร์โว แม้ว่ารูปแบบและยี่ห้อที่ต่างกันของเซอร์โวจะทำให้มีการเปลี่ยนแปลงค่าเล็กน้อย แต่โดยปกติค่าตำแหน่งจะอยู่ระหว่าง 10-40
{% endhint %}

