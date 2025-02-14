<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: 5;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<!-- Title -->
<h1 align="center"><b>CS211.P11 - TRÍ TUỆ NHÂN TẠO NÂNG CAO</b></h1> 


| Student Name        | Student ID |
| ------------------- | ---------- |
|    Hà Huy Hoàng     | 22520460   |


## Danh sách bài tập

### BT1 - Policy Iteration, Truncated Policy Iteration, Value Iteration
- **Mô tả:** Cài đặt và thực nghiệm các thuật toán Policy Iteration, Truncated Policy Iteration và Value Iteration để giải bài toán MDP trên môi trường FrozenLake. So sánh hiệu suất giữa các phương pháp.

### BT2 - SARSA, n-step SARSA, và Q-Learning
- **Mô tả:** Cài đặt các thuật toán học tăng cường SARSA, n-step SARSA và Q-Learning trên môi trường FrozenLake8x8. So sánh reward qua các tập thử nghiệm và phân tích sự khác biệt giữa các thuật toán.

### BT3 - Deep Q-Network (DQN) & Double DQN (DDQN)
- **Mô tả:** Triển khai và so sánh hiệu suất của Deep Q-Network (DQN) và Double DQN (DDQN) trên các môi trường như CartPole-v0 và BreakoutNoFrameskip-v4. Thực hiện tuning hyperparameters và phân tích kết quả.

### BT4 - Deep Deterministic Policy Gradient (DDPG) & Twin-Delayed DDPG (TD3)
- **Mô tả:** Cài đặt và so sánh hai thuật toán DDPG và TD3 trên bài toán điều khiển liên tục với các môi trường như HalfCheetah-v4 và Ant-v4. Đánh giá ảnh hưởng của total timesteps và hyperparameters.

## Chạy BT3 và BT4 trên kaggle
- Đây là repo [cleanrl](https://github.com/l1aF-2027/cleanrl) có sẵn các file cài đặt của các bài trong các folder tương ứng.
- Chạy lần lượt các command dưới đây
```bash
!git clone https://github.com/l1aF-2027/cleanrl.git
%cd cleanrl
!pip install -r requirements/requirements.txt
!pip install -r requirements/requirements-type.txt
!pip install --upgrade typing_extensions
!python cleanrl/algo.py --env-id env --capture_video --seed seed
```
Điền `type`, `algo`, `env` và `seed` cho phù hợp với mỗi lần chạy
