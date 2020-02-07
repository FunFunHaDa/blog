# AWS 기본 사용법 (Windows 10, putty)

## 인스턴스 생성 법

**▼ 아래 사이트에 접속<br>https://aws.amazon.com/ko/console/**  

**▼ 내 계정 => AWS Management Console**
![Image](https://user-images.githubusercontent.com/28629625/74021679-4dcc7100-49df-11ea-95e8-47ae2c3c6664.png)

**▼ EC2**
![Image](https://user-images.githubusercontent.com/28629625/74021249-90417e00-49de-11ea-8dd1-8ea3f493ec5b.png)

**▼ 인스턴스 시작 => 인스턴스 시작**
![Image](https://user-images.githubusercontent.com/28629625/74021300-a2bbb780-49de-11ea-8972-751bd9f37ba4.png)

**▼ 선택 (하고 싶은 운영체제 선택)**
![Image](https://user-images.githubusercontent.com/28629625/74021308-a64f3e80-49de-11ea-9042-20967d445a59.png)

**▼ 다음: 인스턴스 세부 정보 구성**
![Image](https://user-images.githubusercontent.com/28629625/74021315-a8190200-49de-11ea-8656-d866f42254d6.png)

**▼ 다음: 스토리지 추가**
![Image](https://user-images.githubusercontent.com/28629625/74021319-ab13f280-49de-11ea-9d5a-d45af6ce61b0.png)

**▼ 다음: 태그 추가 (필자는 크기 30 지정)**
![Image](https://user-images.githubusercontent.com/28629625/74021325-ae0ee300-49de-11ea-99eb-d22efebcb327.png)

**▼ 다음: 보안 그룹 구성**
![Image](https://user-images.githubusercontent.com/28629625/74021332-b0713d00-49de-11ea-8695-9df14a988c49.png)

**▼ 검토 및 시작 (필자는 8080 Port 추가)**
![Image](https://user-images.githubusercontent.com/28629625/74021336-b2d39700-49de-11ea-97dc-1414b9c941db.png)

**▼ 시작하기**
![Image](https://user-images.githubusercontent.com/28629625/74021343-b535f100-49de-11ea-9553-38b0d583d289.png)

**▼ 새 키 페어 생성 => 키 페어 이름 (지정) => 키 페어 다운로드 => 인스턴스 시작**
**<br>(최초 인스턴스 생성 시 접속에 필요한 키를 만듦)** 
![Image](https://user-images.githubusercontent.com/28629625/74021351-b7984b00-49de-11ea-9c52-e2c7b406d057.png)

**▼ 인스턴스 보기**
![Image](https://user-images.githubusercontent.com/28629625/74021359-ba933b80-49de-11ea-9690-f3f55d42170c.png)

## 인스턴스 종료하는 법

**▼ 인스턴스 => 체크 => 우 클릭 => 인스턴스 상태 => 종료** 
![Image](https://user-images.githubusercontent.com/28629625/74021365-bebf5900-49de-11ea-93cd-bc23365c0459.png)

**▼ 예, 종료**  
![Image](https://user-images.githubusercontent.com/28629625/74021372-c252e000-49de-11ea-8b20-143fc614ae86.png)

## putty에서 AWS 접속하는 법

### funfunhada.pem => funfunhada.ppk로 변환

**▼ 우 클릭 => Run PuTTYgen**  
![Image](https://user-images.githubusercontent.com/28629625/74033666-02738c00-49fa-11ea-8e4c-27e67da36963.png)

**▼ Load**   
![Image](https://user-images.githubusercontent.com/28629625/74033673-06071300-49fa-11ea-9a23-01f442b69b1f.png)

**▼ All Files(`*.*`) => funfunhada.pem => 열기**  
![Image](https://user-images.githubusercontent.com/28629625/74033682-0a333080-49fa-11ea-9c0d-bed115d1c769.png)

**▼ 확인**  
![Image](https://user-images.githubusercontent.com/28629625/74033687-0d2e2100-49fa-11ea-8d7c-8116dfecaff0.png)

**▼ Save private key => 예(Y) (같은 폴더 위치에 .ppk 생성 완료)**   
![Image](https://user-images.githubusercontent.com/28629625/74033696-11f2d500-49fa-11ea-8cd3-d0d5203cd4c2.png)

**▼ putty 실행 => ip 주소 입력**  
![Image](https://user-images.githubusercontent.com/28629625/74033705-15865c00-49fa-11ea-8aca-e827a130f922.png)

**▼ SSH => Auth => Browse... => Open**  
![Image](https://user-images.githubusercontent.com/28629625/74033708-17e8b600-49fa-11ea-9ba1-f96713e1a53b.png)

**▼ 예(Y)**  
![Image](https://user-images.githubusercontent.com/28629625/74033711-1b7c3d00-49fa-11ea-8b78-f619a30d986d.png)

**▼ 접속 성공**  
![Image](https://user-images.githubusercontent.com/28629625/74033715-1e772d80-49fa-11ea-8565-0f971b37b181.png)

### Tips

**▼ Run Pageant**  
![Image](https://user-images.githubusercontent.com/28629625/74033724-220ab480-49fa-11ea-91b0-fe4447693be4.png)

**▼ Add Key => funfunhada.ppk => 열기(O) (키를 자동으로 인증하게 도와준다)**  
![Image](https://user-images.githubusercontent.com/28629625/74033733-259e3b80-49fa-11ea-802e-7b23a0b93bd3.png)




### 관련 
[putty (Windows 10)](https://blog.naver.com/kjhkjh0929/221776472229)

### 참고 
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/putty.html

