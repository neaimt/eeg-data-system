
---

# **EEG Data System**

EEG 데이터를 업로드하고 전처리, 분석 및 예측할 수 있는 시스템입니다.

<img width="1414" alt="KakaoTalk_Photo_2025-02-17-22-02-13" src="https://github.com/user-attachments/assets/ff6a224d-e82a-4735-9864-baeae005253c" />


---

## **프로젝트 클론 및 실행 방법**

### **1. 프로젝트 클론**
터미널에서 프로젝트를 저장할 폴더로 이동한 후, 아래 명령어를 실행합니다.

```bash
git clone https://github.com/neaimt/eeg-data-system.git
```

---

### **2. 가상환경 설정 및 활성화**
프로젝트 폴더로 이동 후 가상환경을 설정하고 활성화합니다.

- **Mac/Linux**:
   ```bash
   cd eeg-data-system
   python3 -m venv venv
   source ./venv/bin/activate
   ```

- **Windows**:
   ```bash
   cd eeg-data-system
   python -m venv venv
   .\venv\Scripts\activate
   ```

---

### **3. 패키지 설치**
프로젝트의 의존 패키지를 설치합니다.

```bash
pip install -r requirements.txt
```

---

### **4. 서버 실행**
다음 명령어로 서버를 실행합니다.

```bash
python app.py
```

터미널에 아래 메시지가 나타나면 성공입니다:

```
Running on http://127.0.0.1:5000
```

브라우저에서 **http://127.0.0.1:5000** 주소로 접속합니다.

---

## **웹페이지 사용 방법**

### **1. EEG 데이터 업로드**
- **기능**: EEG 데이터를 업로드할 수 있습니다.  
- **추가**: 기본으로 제공되는 EEG 데이터 목록을 확인할 수 있습니다.

---

### **2. EEG 데이터 분석**
1. **설정 저장**  
   - 설정 이름을 입력하고 원하는 전처리 방법을 선택한 후 **저장** 버튼을 클릭합니다.

2. **데이터 예측**  
   - EEG 데이터 파일과 저장된 설정을 선택하고 **예측** 버튼을 클릭합니다.  
   - 오른쪽 화면에 **시각화** 및 **모델 결과**가 표시됩니다.

3. **시각화 결과 보기**  
   - **시각화 버튼**을 클릭하면 새로운 페이지에서 결과를 확인할 수 있습니다.

---

### **3. 정확도 테이블**
- 모델 성능에 대한 정확도 결과를 테이블 형식으로 확인할 수 있습니다.

---

### **4. 설명 가능한 AI (XAI)**
- 모델 예측 결과를 설명하는 시각화 도구를 제공합니다.

---

## **프로젝트 구조**
```
eeg-data-system/
│
├── app.py                   # 서버 실행 메인 파일
├── requirements.txt         # 패키지 의존성 파일
├── templates/               # HTML 파일
├── static/                  # CSS, JavaScript 및 정적 파일
├── data/                    # 기본 EEG 데이터
└── README.md                # 프로젝트 설명 파일
```

---

## **기타 사항**
- 서버 실행 시 Python 3.8 이상을 권장합니다.  
- 이 시스템은 기본 EEG 데이터셋을 제공하며, 사용자가 추가 데이터를 업로드하여 분석할 수 있습니다.

---

**이제 프로젝트를 실행하고 EEG 데이터를 분석해보세요! 🚀**

---
