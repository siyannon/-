# -
可通过在kali上运行脚本，测试邮箱的SPF是否有效，如果无效，那就有可能被伪造邮箱进行钓鱼
This is a Kali script.
#!/bin/bash

while IFS= read -r line; do
  swaks --body "Hacked by siyannon " --header "Subject: $line Hacker" --h-From: "$line <notify@$line>" -f notify@$line -t  siyannonxxx@163.com --header-X-Mailer $line
done < domain.txt  ![image](https://github.com/siyannon/-/assets/164863911/081e6465-970d-47ac-bcd1-e8456376a4d2)


By running the above script, the specified content within the script will be sent to the designated email address.
![屏幕截图(113)](https://github.com/siyannon/-/assets/164863911/fb93ec99-140a-42c5-a960-129b3c416fe5)
![屏幕截图(112)](https://github.com/siyannon/-/assets/164863911/10015c6d-ab6e-4a24-9e26-aa807cda4b46)


