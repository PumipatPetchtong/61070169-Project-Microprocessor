# 🛠 Project-Microprocessor Raspberry pi-61070169 🛠
<h2>🚪 Camera security (กล้องติดหน้าห้อง)</h2><br>
  ในปัจจุบันความปลอดภัยเป็นสิ่งที่สำคัญ โปรเจคนี้จึงได้ออกแบบความปอดภัยสำหรับคนที่อยู่ห้องคนเดียวหรือหลายคนก็ได้ โดยโปรเจคนี้จะใช้ Raspberry pi กับ ตัวกล้อง ในการติดที่ประตูห้องหรือตามผนังหน้าห้องเพื่อ
  ที่จะดูว่ามีใครมาหาหรือมีใครเคาะประตูเวลาที่เราอยู่ห้องโดยที่ตัวเราเองไม่ต้องเปิดประตูออกไปดูและเพื่อความปอดภัยของตัวเอง เครื่องมือสามารถดูภาพได้แบบ real time ดูได้ตลอดเมื่อเข้าไปเชคดู<br>
<h2>🔧 Device</h2>
<html>
<head>
</head>
<body>
<table>
  <tr>
    <th>Raspberry Pi</th>
    <th>Camera</th>
  </tr>
  <tr>
    <td><img src="https://asset.conrad.com/media10/isa/160267/c1/-/en/002138864PI00/image.jpg"width="700" height="400"></td>
    <td><img src="https://i.postimg.cc/HnSzDhVX/camera.jpg"width="500" height="400"></td>
  </tr>
</table>
</body>
</html>

<h2>⚙️ Configuration</h2>
1. ติดตั้งกล้อง Camera pi <br>
   - โดยการใช้คำสั่ง pi@raspberry:~ $ sudo raspi-config <br>
   - เลือกในส่วนของ Interfacing Options<br>
   - แล้วทำการ enable camera <br>
   - กดเลือก Finish<br><br>
2. ใช้คำสั่ง pi@raspberry:~ $ ifconfig เพื่อดูว่าเราต้องใช้ ip เบอร์อะไรเพื่อที่จะเข้าไปดู live ในเว็บบราวเซอร์<br><br>
    <img src="https://i.postimg.cc/6pDk3Npc/1621613200235.jpg"width="500" height="400"><br>
3. ใช้คำสั่ง pi@raspberrypi:~ $ sudo apt-get install python-picamera python3-picamera พื่อติดตั้ง python pi camera<br><br>
4. ใช้คำสั่ง pi@raspberrypi:~ $ nano rpi_camera_surveillance_system.py เพื่อเขียนโค๊ตโดยใช้ภาษา Python<br><br>
5. ใช้คำสั่ง pi@raspberrypi:~ $ python3 rpi_camera_surveillance_system.py เพื่อรันโค๊ต<br><br>
6. ไปที่หน้า Web browser แล้วทำการใส่ ip address ในตอนแรก http://192.168.1.58:8000<br><br>
    <img src="https://i.postimg.cc/HWwhsJrP/message-Image-1621614404202.jpg"width="500" height="300"><br><br>
** โปรเจคกล้อง Raspberry pi ตัวนี้สามารถนำไปเป็นกล้อง Wedcam ใช้สำหรับกล้องคอมพิวเตอร์ได้อีกด้วย
