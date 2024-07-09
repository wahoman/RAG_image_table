pdf에 있는 이미지, 표까지 읽고 답변해주는 챗봇

## 7/5  

테디노트 참고중

임베딩 여러번하다가 5달러 다써버림; -0.43달러 달성. 지원해달라고 해야댐

## 7/9 

메뉴얼 기반 챗봇인데 단순하게 csv 파일로 예상 질문과 답변 만들어서 할까 고민중

3가지 방법 비교

---

## 모델 비교

| **항목**          | **CSV 파일 기반 Q&A 시스템**                                               | **오픈소스 모델**                                                                 | **OpenAI 모델**                                                                  |
|-------------------|---------------------------------------------------------------------|------------------------------------------------------------------------------|------------------------------------------------------------------------------|
| **비용**   | 추가적인 API 호출 비용이 없음                                           | 무료로 사용할 수 있으나, 하드웨어와 인프라 비용이 발생할 수 있음                          | API 호출에 대한 비용이 발생하며, 사용량이 많을수록 비용이 증가                                      |
| **속도**| 미리 정의된 답변을 제공하므로 응답 속도가 매우 빠름                                | 하드웨어 성능에 따라 시간이 오래 걸릴 수 있음                                                | 강력한 API로 빠른 응답이 가능하지만 네트워크 지연이 있을 수 있음                                    |
| **구현**   | 구현이 간단하며, 복잡한 모델이나 하드웨어가 필요 없음                                | 모델 설정과 유지보수가 필요함                                                      | API 호출만으로 강력한 기능을 사용할 수 있어 구현이 비교적 쉬움                                     |
| **보안**    | 모든 데이터가 로컬에 저장되므로 민감한 데이터가 외부로 유출되지 않음                         | 데이터가 로컬에서 처리되므로 프라이버시가 강화됨                                           | 데이터를 외부 API로 전송해야 하므로 데이터 프라이버시가 우려될 수 있음                                  |
| **유연성**   | 예상하지 못한 질문이나 복잡한 질문에 대해 적절한 답변을 제공하기 어려움                       | 모델의 구조와 파라미터를 수정할 수 있어 유연성이 높음                                        | 대규모 학습 데이터와 강력한 성능으로 유연성이 높음                                                  |
| **유지보수**      | 새로운 질문이 생길 때마다 CSV 파일을 업데이트해야 하므로 유지보수가 필요                     | 최신 연구 결과를 반영한 업데이트를 직접 수행해야 함                                       | OpenAI가 모델을 지속적으로 개선하고 업데이트하므로 유지보수가 용이함                                |
| **정확도**   | 질문과 답변 매칭이 정확하지 않을 수 있으며, 유사도가 낮은 경우 정확한 답변을 제공하기 어려움   | 최신 상업용 모델만큼의 성능을 기대하기 어려울 수 있음                                       | 대규모 학습 데이터와 강력한 성능으로 높은 정확도를 제공함                                           |

유연성이나 유지보수 측면이 우려가 되긴 하지만, 새로운 정보가 계속해서 업데이트 되는 것이 아닌 정해진 메뉴얼을 바탕으로 질문이 들어오고 답변이 나가기 때문에 CSV 파일 기반 챗봇 시스템에서 큰 문제가 되지 않을 것이라고 생각.

---
