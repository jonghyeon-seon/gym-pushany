<<<<<<< HEAD
# example.py
import gymnasium as gym
import anypush

env = gym.make("'anypush/AnyPush-v0'", render_mode="human")
observation, info = env.reset()

for _ in range(1000):
    action = env.action_space.sample()
    observation, reward, terminated, truncated, info = env.step(action)
    image = env.render()

    if terminated or truncated:
        observation, info = env.reset()

env.close()
=======
## AnyPush
>>>>>>> 0dc1b9c (working!)
