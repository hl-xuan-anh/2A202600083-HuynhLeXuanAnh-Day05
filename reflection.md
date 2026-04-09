# Reflection – Hackathon

## 1. Role cụ thể trong nhóm
- Research về product XanhSM và nghiên cứu pain point người dùng.
- Là người chuyển yêu cầu bài toán thành flow rõ ràng cho chatbot
- Thiết kế cách AI hiểu input người dùng (prompt + logic).
- Phối hợp với teammate để đảm bảo AI gọi đúng tool và trả output hợp lý.
- Tổng hợp các document phân tích.
---

## 2. Phần phụ trách cụ thể
Các đóng góp chính có output rõ ràng:

- **Phân tích AI chatbot thành 6 document tổng hợp thành spec**
  → Output: 6 phần chi tiết của spec

- **Cùng viết và tối ưu prompt cho AI**
  → Output: bộ prompt chính + các rule để AI không trả lời sai format

- **Định nghĩa test case cho chatbot**
  → Output: danh sách test case gồm đúng / sai / ambiguous để kiểm tra hành vi AI

---

## 3. SPEC: mạnh nhất & yếu nhất

**Mạnh nhất:**
- Phần **User Stories**
  → Vì nhóm xác định rõ được các path AI xử lý hợp lý ngay từ đầu  
  → Xác định được các feature chính của nhóm.

**Yếu nhất:**
- Phần **Eval metrics & threshold**
  → Vì chưa có kinh nghiệm đặt ra threshold thực tế

---

## 4. Đóng góp khác (ngoài phần chính)
- Test prompt với nhiều kiểu input khác nhau (người dùng viết sai chính tả, thiếu thông tin…)
- Support team chỉnh lại logic khi AI trả lời không đúng expectation

---

## 5. 1 điều học được (trước đó chưa biết)
Tôi học được rằng:

> **AI không “hiểu” như con người — nó chỉ làm đúng nếu mình mô tả cực kỳ rõ.**

Trước đây tôi nghĩ prompt chỉ cần viết “tương đối”, nhưng thực tế:
- Nếu không define rõ rule → AI sẽ tự đoán
- Và thường đoán sai trong edge cases
- Càng viết chi tiết thì AI xử lý các case càng mượt

---

## 6. Nếu làm lại, tôi sẽ đổi gì?
Cụ thể:
- **Tách prompt thành nhiều phần nhỏ (system / instruction / examples)** thay vì nhồi vào 1 prompt lớn

---

## 7. AI giúp gì? AI sai ở đâu?

**AI giúp:**
- Generate nhanh idea flow và cách xử lý tình huống
- Viết base prompt và code nhanh hơn
- Hỗ trợ debug logic khi bị stuck

**AI sai / mislead:**
- Đôi khi **suggest logic sai nhưng nghe rất hợp lý**
- Không tự nhận ra thiếu edge case
- Có lúc **không tuân thủ instruction (không gọi tool, trả sai format)** dù prompt đã ghi

→ Kết luận:  
AI rất mạnh để tăng tốc, nhưng **không thể tin hoàn toàn**, vẫn cần người kiểm soát logic.

---