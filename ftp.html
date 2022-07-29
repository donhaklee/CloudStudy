## **FTP**

**1) FTP 서버 운영**

**\- MobaXterm으로 접근**

[##_Image|kage@dkEggz/btrIt9fsHgr/nuVC373kQnhZARl24PhSp0/img.png|CDM|1.3|{"originWidth":1161,"originHeight":712,"style":"alignCenter","width":757,"height":464}_##]

-   **여러 사이트가 Public하게 Open License를 제공한다.**
-   **파일 공유를 메일없이 운영 가능하다.**
-   **현재는 보안문제와 구글 드라이브와 같은 대체품이 있어 잘 사용하지 않는다.**

**2) FTP 운영모드**

**\- TCP port range**

-   **system port : 1 - 1023 : service (Daemon)**
-   **user port : 1024 - 49151**
-   **private port : 49152 - 65535**

[##_Image|kage@bVGaJM/btrIt46Cyuv/SMX0x90WKZPRbC9f6L6PYK/img.png|CDM|1.3|{"originWidth":963,"originHeight":515,"style":"alignCenter","width":800,"height":428}_##]

**\- Active Mode : 고정**

-   **Control port 21번(연결할 때)**
-   **Data port 20번 (클라이언트가 데이터를 다운받을 때)**
-   **1 ~ 2 :클라이언트가 서버에게 21번으로 요청해 3-way-handshake (21과 클라이언트 연결)로 tcp연결를 하지만 그 과정에서 클라이언트는 어떤 포트로 데이터를 받을지 랜덤한 번호로 보낸다. 그렇기에 모든 포트가 열려있어야 가능하고 클라이언트가 방화벽 관리를 해야한다.**
-   **3 ~ 4 : 서버는 미리 알려준 클라이언트 포트로 요청, 클라이언트 응답**

**\- Passive Mode : 가변**

-   **Control port 21번(연결할 때)**
-   **Data port ?번 (클라이언트가 데이터를 다운받을 때)**
-   ****서버에서 데이터를 보낼 포트를 미리 정하고 클라이언트도 특정 포트로 요청을 보내기 때문에 서버가 방화벽 관리를 하면되고 클라이언트도 안전하게 정보교환이 가능하다.****

[##_Image|kage@cCMhQd/btrIq5ynCYW/lapndMZElMhjJzkuqPRty1/img.png|CDM|1.3|{"originWidth":1276,"originHeight":703,"style":"alignCenter","width":791,"height":436}_##]

-   **사이트가 두 가지 모드 중 하나만 운영하면 접근되지 않는다.**

**3) 인증별 FTP 운영**

**\- 익명 사용자 전용 : 공개용 FTP**

-   **ID : anonymous**
-   **PWD : @ or anonymous**
-   **read only**

**\- 로컬 사용자 전용 : 개인용 FTP**

-   **ID : /etc/passwd**
-   **read only 또는 read write를 결정해야한다 (read write는 프로젝트를 운영할 때 사용한다.)**

**\- 익명/로컬 사용자 전용**

**4) 설치**

```
yum -y install vsftpd
cd /etc/vsftpd/
vim vsftpd.conf # 설정
```

```
systemctl enable --now vsftpd
firewall-cmd --reload
firewall-cmd --list-services
firewall-cmd 


[root@client vsftpd] cat /etc/passwd | egrep ftp
ftp:x:14:50:FTP User:/var/ftp:/sbin/nologin  # ftp 홈 디렉토리
```

[##_Image|kage@BuZ1J/btrIn5eUsLA/0jAhY2BHxs09K5XLHKVVb1/img.png|CDM|1.3|{"originWidth":642,"originHeight":247,"style":"alignCenter","width":559,"height":215}_##]

```
cp /etc/yum.conf ./   # 익명사용자들은 ftp의 홈디렉토리로 들어온다
```

[##_Image|kage@renJx/btrIsen5Cj7/6xXOKE8vOWQjknSIYQkK1K/img.png|CDM|1.3|{"originWidth":718,"originHeight":171,"style":"alignCenter","caption":"생성된 yum.conf"}_##][##_Image|kage@bEDn0w/btrIwHQsheU/bfwhI2Hx9FuaZRlDdugdn0/img.png|CDM|1.3|{"originWidth":439,"originHeight":88,"style":"alignCenter","caption":"하지만 기본적으로 others에겐 w가 없어 ftp에 디렉터리를 생성할 수 없다"}_##]

**\- others에게 로컬 디렉터리의 권한 허용**

```
chmod o+w /var/ftp/pub
```

[##_Image|kage@bw0Mv5/btrIwGKL6Cl/Za7byAbYYbiCUiEqjI35Sk/img.png|CDM|1.3|{"originWidth":517,"originHeight":82,"style":"alignCenter","caption":"그래도 만들어지지 않는다."}_##]

**\- 익명에게 daemon 권한 허용**

```
[root@client ftp] vim /etc/vsftpd/vsftpd.conf
[root@client ftp] systemctl restart vsftpd
setenforce 0
```

[##_ImageGrid|kage@CBz6o/btrIoAsjM6p/nyI8pwP0lcaFNfkPbSosb0/img.png,kage@bcblKO/btrIq6dar3U/LJ6wcBL62SVF1YsnXfZTok/img.png|data-origin-width="289" data-origin-height="111" data-is-animation="false" style="width: 52.1994%; margin-right: 10px;" data-widthpercent="52.81",data-origin-width="435" data-origin-height="187" data-is-animation="false" data-widthpercent="47.19" style="width: 46.6378%;"|_##]

-   **로컬 디렉터리의 퍼미션과 daemon설정과 같이 설정되어야한다.**
-   **로컬에서의 권한과 daemon 권한 둘 다 허용되어야 디렉터리가 생성된다.**

[##_ImageGrid|kage@VAekh/btrImc6atER/aWkdO7yIvAJuA98AHAFDkk/img.png,kage@BpbSX/btrIn4AkAIx/X2Qc64wlUKAXVjNUPgTU5K/img.png|data-origin-width="292" data-origin-height="117" data-is-animation="false" style="width: 54.8001%; margin-right: 10px;" data-widthpercent="55.44",data-origin-width="361" data-origin-height="180" data-is-animation="false" data-widthpercent="44.56" style="width: 44.0371%;"|pc의 파일도 업로드도 가능하다_##]

**\- 로컬 사용자에서 파일을 생성해도 가능하다**

```
cd /home/centos
```

**5) chroot : change root**

[##_Image|kage@dh4xZv/btrIoI4jLc3/XI9kXphABvgvkIyMinQ3z0/img.png|CDM|1.3|{"originWidth":655,"originHeight":174,"style":"alignCenter","caption":"allow_writeable_chroot=YES을 추가해야한다"}_##]

```
1) 모든 사용자를 홈디렉터리로 제한
chroot_local_user=YES
# chroot_list_enable=YES
# chroot_list_file=/etc/vsftpd/chroot_list
allow_writeable_chroot=YES

2) chroot_list에 등록된 로컬 사용자의 접속을 자신의 홈 디렉터리로 제한
# chroot_local_user=YES
chroot_list_enable=YES
chroot_list_file=/etc/vsftpd/chroot_list
allow_writeable_chroot=YES

3) chroot_list에 등록되지 않은 로컬 사용자의 접속을 자신의 홈 디렉터리로 제한
chroot_local_user=YES
chroot_list_enable=YES
chroot_list_file=/etc/vsftpd/chroot_list
allow_writeable_chroot=YES

4) chroot_local_user의 기본값은 no이다.
```

```
vim /etc/vsftpd/chroot_list # centos 입력
```

-   **모든 사용자가 /로 이동할 수 있는 문제를 해결하기 위해 사용자에게 최상위 계층을 정해주는 것이다.**
-   **list\_enable = yes는 listfile에 있는 사람들만 제한할 수 있다.**
-   **centos는 본인의 /home/centos를 최상위 계층인 /로 인식하게 돼서 최상위 계층을 보호할 수 있다.**

**\- 확인**

```
yum -y install ftp
ftp 192.168.108.5
```

[##_ImageGrid|kage@bZZoq8/btrIsRfQUy1/ZiYWY6XL5kvLkaGVIKYKK0/img.png,kage@bMHVYn/btrIuYyyr4k/PlFKD6ViAz1ZZwt5fKbrYk/img.png|data-origin-width="348" data-origin-height="196" data-is-animation="false" data-widthpercent="45.85" style="width: 45.3125%; margin-right: 10px;",data-origin-width="388" data-origin-height="185" data-is-animation="false" data-widthpercent="54.15" style="width: 53.5247%;"|(왼) 적용 전 (오) 적용 후 =&gt; 2)로 적용_##][##_ImageGrid|kage@ubyHb/btrIvnY0Fyp/mFeQm86AKjMMuugKIjDqLk/img.png,kage@b2TShB/btrIn05h35t/yC2m5kL92HPCMVbfC7t6n0/img.png|data-origin-width="689" data-origin-height="323" data-is-animation="false" style="width: 46.2848%; margin-right: 10px;" data-widthpercent="46.83",data-origin-width="683" data-origin-height="282" data-is-animation="false" style="width: 52.5524%;" data-widthpercent="53.17"|(왼) 적용 전 (오) 적용 후 =&gt; 적용된 상태로는 실제 root디렉터리로 접근할 수 없게 된다._##]
