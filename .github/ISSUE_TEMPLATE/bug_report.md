name: แจ้งปัญหา (Bug Report)
description: แจ้งข้อผิดพลาดหรือปัญหาที่พบในปลั๊กอิน
title: "[Bug] "
labels:
  - bug

body:
  - type: markdown
    attributes:
      value: |
        ## ขอบคุณที่ช่วยแจ้งปัญหา ❤️
        กรุณากรอกข้อมูลให้ครบเพื่อให้เราตรวจสอบได้รวดเร็วยิ่งขึ้น

  - type: input
    id: plugin_version
    attributes:
      label: เวอร์ชันของปลั๊กอิน
      placeholder: เช่น 1.0.0
    validations:
      required: true

  - type: input
    id: mc_version
    attributes:
      label: เวอร์ชัน Minecraft
      placeholder: เช่น 1.21.8
    validations:
      required: true

  - type: input
    id: server
    attributes:
      label: เซิร์ฟเวอร์ที่ใช้
      placeholder: เช่น Paper, Purpur, Folia
    validations:
      required: true

  - type: textarea
    id: description
    attributes:
      label: อธิบายปัญหา
      description: อธิบายว่าเกิดอะไรขึ้น
    validations:
      required: true

  - type: textarea
    id: reproduce
    attributes:
      label: วิธีทำให้เกิดปัญหา
      placeholder: |
        1. ทำ...
        2. ใช้คำสั่ง...
        3. เกิดปัญหา...
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: ผลลัพธ์ที่คาดหวัง
      description: ควรจะเกิดอะไรขึ้น
    validations:
      required: true

  - type: textarea
    id: logs
    attributes:
      label: Log / Error
      description: แนบข้อความ Error หรือ Log ทั้งหมด
      render: shell

  - type: textarea
    id: plugins
    attributes:
      label: ปลั๊กอินอื่นที่ติดตั้ง
      placeholder: |
        - EssentialsX
        - LuckPerms
        - PlaceholderAPI

  - type: textarea
    id: additional
    attributes:
      label: ข้อมูลเพิ่มเติม
      description: เช่น รูปภาพ วิดีโอ หรือไฟล์ config
