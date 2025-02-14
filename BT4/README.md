# Bài tập 4 - Deep Deterministic Policy Gradient (DDPG) & Twin-Delayed DDPG (TD3)  

---

Chào cả lớp,  

Trong bài tập thực hành này, chúng ta cần cài đặt và so sánh hiệu năng của **DDPG** và **TD3** cho **bài toán điều khiển liên tục (continuous control)**.  
Để thuận tiện cho việc thực nghiệm, chúng ta có thể sử dụng **CleanRL framework**:  
🔗 [CleanRL Github](https://github.com/vwxyzjn/cleanrl)  

### **Cài đặt CleanRL**:
```bash
git clone https://github.com/vwxyzjn/cleanrl.git && cd cleanrl
pip install -r requirements/requirements.txt
pip install -e .
```
CleanRL được thiết kế để mỗi thuật toán có thể được thực thi chỉ bằng **1 file duy nhất**.  

Ví dụ để chạy thuật toán **DDPG** hoặc **TD3** cho **Hopper-v4**:  
```bash
python cleanrl/ddpg_continuous_action.py --env-id Hopper-v4 --capture_video --seed 1
python cleanrl/td3_continuous_action.py --env-id Hopper-v4 --capture_video --seed 1
```
Kết quả thực nghiệm được lưu lại với **Tensorboard** (trong thư mục `runs/`), và video được phát sinh (nếu có `--capture_video`) được lưu trong thư mục `videos`.  

---

## **Yêu cầu bài tập**  

Trong bài tập này, chúng ta cần hoàn thành **các nội dung sau**:  

✅ **Thực nghiệm và đánh giá hiệu năng**  
- Huấn luyện và so sánh **DDPG** và **TD3** trên **HalfCheetah-v4** (với **3 random seeds**: `MSSV1`, `MSSV2`, `MSSV3` - mỗi MSSV là mã số sinh viên của bạn).  
- Huấn luyện và so sánh **DDPG** và **TD3** trên **Ant-v4** (với **3 random seeds**: `MSSV1`, `MSSV2`, `MSSV3`).  

✅ **Phân tích kết quả**  
- Vẽ đồ thị **reward** của DDPG và TD3 trên cả hai môi trường.  
- Đánh giá hiệu năng của **TD3** so với **DDPG** dựa trên đồ thị thu thập trong từng cột độ thị cho mỗi tác vụ (**HalfCheetah-v4** và **Ant-v4**).  

✅ **Thiết lập số tập huấn luyện hợp lý**  
- **total timesteps** lớn hơn **1.000.000** (có thể thử tăng thêm để đạt hiệu quả huấn luyện tốt hơn).  
- Có thể **tải MuJoCo** để có thể mô phỏng các bài toán điều khiển liên tục tốt hơn.  

📌 **Gợi ý:** Nếu gặp lỗi khi chạy **Ant-v4**, bạn có thể thử thay thế bằng **HalfCheetah-v2** hoặc **Ant-v2**.  

---

## **Bài nộp**  

📌 **1 file ipynb** báo cáo kết quả thực nghiệm (**gồm mã nguồn huấn luyện** cho cả DDPG và TD3).  
📌 **Trình bày ngắn gọn sự khác nhau giữa cơ chế hoạt động của DDPG và TD3**.  
📌 **Các file video được phát sinh sau khi thuật toán huấn luyện** (có thể tải lên Google Drive và đính kèm link vào báo cáo).  

📝 **Nộp bài bằng 1 file zip** đặt tên theo **BT4_MSSV.zip**.  
⏳ **Deadline: 12/01/2025** (Bài nộp sau ngày này sẽ bị tính điểm trễ hạn). **Từ ngày 19/01/2025 sẽ không chấm thêm bài nộp mới**.  

---

## **Tham khảo**  

🔗 DDPG và TD3 trên **DeepMind**:  
- [https://docs.cleanrl.dev/rl-algorithms/ddpg](https://docs.cleanrl.dev/rl-algorithms/ddpg)  
- [https://docs.cleanrl.dev/rl-algorithms/td3](https://docs.cleanrl.dev/rl-algorithms/td3)  
- [https://spinningup.openai.com/en/latest/algorithms/ddpg.html](https://spinningup.openai.com/en/latest/algorithms/ddpg.html)  
- [https://spinningup.openai.com/en/latest/algorithms/td3.html](https://spinningup.openai.com/en/latest/algorithms/td3.html)  
