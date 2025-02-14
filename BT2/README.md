# Bài tập 2 - SARSA, n-step SARSA, and Q-Learning  
---

Chào cả lớp,  

Trong bài tập này chúng ta cần cài đặt, thực nghiệm, và nhận xét kết quả thực nghiệm của:  

1. **SARSA** (đã có phần cài đặt gợi ý trong file ipynb đính kèm).  
2. **n-step SARSA**: tự cài đặt, tự thực nghiệm với một vài giá trị của `n` tự chọn.  
3. **Q-Learning**: tự cài đặt.  

### Với 3 thuật toán trên, chúng ta cần thực nghiệm với các tổ hợp:
- Môi trường `FrozenLake` và `FrozenLake8x8`.  
- Discount factor `gamma = 0.9` và `gamma = 1.0`.  
- Tham số `is_slippery`: `False` và `True`.  

> **Lưu ý:** các siêu tham số như **learning rate alpha** và **số tập (num_episodes)** có thể cần phải tinh chỉnh cho phù hợp với mỗi môi trường và thuật toán.  

### Để so sánh hiệu năng của các thuật toán SARSA, n-step SARSA và Q-Learning thì nên:
- Vẽ đồ thị **reward** của 3 thuật toán trong cùng 1 đồ thị.  
- Vẽ đồ thị **episode length** của 3 thuật toán trong cùng 1 đồ thị.  

Các kết quả thực nghiệm, đồ thị kết quả, chiến lược tối ưu tìm được, và các nhận xét về kết quả thực nghiệm chúng ta trình bày trong file ipynb.  
File ipynb phải thể hiện được kết quả chạy thực nghiệm.  

**Bài nộp:** gồm 1 file ipynb duy nhất đặt tên `BT2_MSSV.ipynb` với MSSV là mã số sinh viên của bạn.  
