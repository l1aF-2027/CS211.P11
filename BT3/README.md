# Bài tập 3 - Deep Q-Network (DQN) & Double DQN (DDQN)  


Chào cả lớp,  

Trong bài tập thực hành này chúng ta cần cài đặt và so sánh hiệu năng của **Deep Q-Network (DQN)** và **Double DQN (DDQN)**.  
Để thuận tiện cho việc thực nghiệm, chúng ta có thể sử dụng **CleanRL framework**:  
🔗 [CleanRL Github](https://github.com/vwxyzjn/cleanrl)  

### Cài đặt CleanRL:
```bash
git clone https://github.com/vwxyzjn/cleanrl.git && cd cleanrl
pip install -r requirements/requirements.txt
pip install -e .
```
CleanRL được thiết kế để mô hình huấn luyện có thể được thực thi chỉ bằng **1 file duy nhất**.  

Ví dụ để chạy thuật toán **DQN** cho **CartPole-v0**:  
```bash
python cleanrl/dqn.py --seed 1 --total-timesteps 50000 --capture_video
```
Để chạy **DQN cho game Atari** (ví dụ **BreakoutNoFrameskip-v4**):  
```bash
python cleanrl/dqn_atari.py --seed 1 --env-id BreakoutNoFrameskip-v4 --total-timesteps 1000000 --capture_video
```
Kết quả thực nghiệm được lưu lại với **Tensorboard**, trong thư mục `runs/`, và video được phát sinh trong `runs/{experiment_name}/videos`.  

---

## **Yêu cầu bài tập**  

Trong bài tập này, chúng ta cần hoàn thành **các nội dung sau**:  

✅ **Cài đặt thuật toán Double DQN (DDQN)**  
- Dựa trên mã nguồn DQN của CleanRL, cài đặt thuật toán **Double DQN**.  
- Huấn luyện và so sánh **DQN** và **Double DQN** trên **CartPole-v0** (với **3 random seeds**: `MSSV1`, `MSSV2`, `MSSV3` - mỗi MSSV là mã số sinh viên của bạn).  
- Huấn luyện và so sánh **DQN** và **Double DQN** trên **BreakoutNoFrameskip-v4** (với **3 random seeds**: `MSSV1`, `MSSV2`, `MSSV3`).  

✅ **Thực nghiệm và đánh giá**  
- Vẽ đồ thị **reward** và **số bước (episode length)** của DQN và Double DQN trên cả hai môi trường.  
- Đánh giá hiệu năng của **Double DQN** so với **DQN**.  

✅ **Thiết lập số tập huấn luyện hợp lý**  
- Với **CartPole-v0**, tổng số tập huấn luyện (**total-timesteps**) cần lớn hơn `50.000`.  
- Với **BreakoutNoFrameskip-v4**, tổng số tập huấn luyện (**total-timesteps**) cần lớn hơn `1.000.000`.  

---

## **Bài nộp**  

📌 **1 file ipynb** báo cáo kết quả thực nghiệm (**gồm mã nguồn huấn luyện** cho cả DQN và Double DQN).  
📌 **Trình bày ngắn gọn sự khác nhau giữa cơ chế hoạt động của DQN và Double DQN**.  
📌 **Các file video được phát sinh sau khi thuật toán huấn luyện** (có thể tải lên Google Drive và đính kèm link vào báo cáo).  

📝 **Nộp bài bằng 1 file zip** đặt tên theo **BT3_MSSV.zip**.  
⏳ **Deadline: 15/12/2024** (Bài nộp sau ngày này sẽ bị tính điểm trễ hạn). **Từ ngày 22/12 sẽ không chấm thêm bài nộp mới**.  

---

## **Tham khảo**  

🔗 Double DQN trên **DeepMind**:  
- [https://arxiv.org/abs/1509.06461](https://arxiv.org/abs/1509.06461)  
- [https://adityashrm21.github.io/papers/DQN_paper.pdf](https://adityashrm21.github.io/papers/DQN_paper.pdf)  
- [https://uvadlc-notebooks.readthedocs.io/en/latest/tutorial_notebooks/reinforcement_learning/Deep_Q_Network.html](https://uvadlc-notebooks.readthedocs.io/en/latest/tutorial_notebooks/reinforcement_learning/Deep_Q_Network.html)  
