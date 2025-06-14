# Chat GPT를 활용한 AI음성 수화 번역 서비스
## 📘 프로젝트 소개
수어 통역사의 수가 부족한 상황에서, 농인의 정보 접근권을 보장하기 위한 기술적 대안이 필요합니다.

본 프로젝트는 영상 속 자연어 문장을 인공지능 기반으로 분석하여, 이를 아바타 수어로 실시간 변환함으로써 농인의 매체 내용 이해를 돕는 시스템을 구축하는 것을 목표로 합니다.
<br>
<br>

## 🎯 프로젝트 목적
- 구어를 입력받아 텍스트 분석을 통해 AI로 수어를 자동 생성하여 모션 캡쳐 등의 불필요한 과정을 최소화한 서비스 제공
- 일반 텍스트의 수어 표현 문장으로의 변환
- 구어를 실시간으로 번역하여, 시간과 공간의 제약 없이 아바타를 통해 다양한 매체 활용 가능
- 수어 데이터 선정, 데이터 수집, 데이터 정제 및 구체화, 데이터 증식을 통한 데이터의 전처리 완성
- 정확한 딥러닝 알고리즘(StableDiffusion, ControlNet 등)과 전이학습, 데이터 검수 등을 통해 최종 모델 선정으로 높은 성능의 수어 동작 생성
<br>
<br>

## 🧾 System Configuration
유즈케이스는 아래와 같습니다.
![유즈케이스](https://github.com/user-attachments/assets/4ed24257-0ea8-404f-bbbd-c1cfbaf87d03)



<br>
<br>

## 📘 E-R Diagram
![엔티티](https://github.com/user-attachments/assets/2f12fdaf-0db0-4cf9-9a98-8aaca997d69e)


<br>
<br>

## 🗂️ 주요 기능
- **음성 인식**: OpenAI Whisper API를 활용하여 음성을 텍스트로 자동 변환
- **말뭉치 데이터 증강**: GPT 기반 데이터 증강을 통해 수어 문장 구조에 맞는 다양한 문장 생성
- **한국어-수어 변환**: Transformer기반 모델(KoBART)을 이용해 한국어 문장을 수어 문법 구조로 변환
- **수어 포즈 추출**: DWPose를 활용하여 아바타 생성용 포즈(Keypoints) 자동 추출
- **수어 아바타 생성**: Stable Diffusion과 ControlNet을 이용해 추출된 포즈 기반 수어 아바타 이미지 생성
<br>
<br>


## ⚙️ Tech Stack
| 항목 | 사용 기술 |
|------|-----------|
| 언어 | Python, Dart |
| 프레임워크 / 라이브러리 | TensorFlow, Keras, Pandas, NumPy, OpenCV, Transformers, DWPose, Stable Diffusion, ControlNet |
| 모델 | OpenAI Whisper (음성 인식), GPT (데이터 증강), Transformer (수어 변환), DWPose (포즈 추출), Stable Diffusion + ControlNet (수어 아바타 생성) |
| 개발 환경 | Windows, Ubuntu, Visual Studio Code, Google Colab, ComfyUI |
| 데이터베이스 | Firebase |
| 서버 / 인프라 | AWS EC2, Docker, FastAPI |
| 모바일 개발 | Flutter (Dart 기반) |

<br>
<br>

## 📚 세부 기능별 README 및 Repository 링크
|  README 링크                                                                                                                   |  GitHub Repository                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------- |
| [Speech2SignTranslation - README.md](https://github.com/Speech2KSL-AvatarGenerator/Speech2SignTranslation/blob/main/README.md) | [Speech2SignTranslation](https://github.com/Speech2KSL-AvatarGenerator/Speech2SignTranslation) |
| [SignAvatarGeneration - README.md](https://github.com/Speech2KSL-AvatarGenerator/SignAvatarGeneration/blob/main/README.md)     | [SignAvatarGeneration](https://github.com/Speech2KSL-AvatarGenerator/SignAvatarGeneration)     |
| [SignAvatarApp-suddy - README.md](https://github.com/Speech2KSL-AvatarGenerator/SignAvatarApp-suddy/blob/main/README.md)       | [SignAvatarApp-suddy](https://github.com/Speech2KSL-AvatarGenerator/SignAvatarApp-suddy)       |

