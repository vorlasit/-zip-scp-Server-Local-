#  ตัวอย่าง: zip + scp ขณะส่งไฟล์ (จาก Server → Local)
      ssh bfsvr@10.150.1.52 "zip -r - /opt/odoo/.local/share/Odoo/filestore/reallivekkm3223" > reallivekkm3223_filestore.zip

# ตัวอย่าง: zip + scp ขณะส่งไฟล์ (จาก Local → Server)
      zip -r - ./folder_from_local | ssh bfsvr@10.150.1.52 "cat > /path/ubuntuserver/myproject.zip"
# Allow all user like owner
      sudo chmod 777 -R customized
