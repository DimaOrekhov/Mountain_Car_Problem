# Mountain_Car_Problem

Для задачи MountainCar-v0 с дискретным action space лучшее решение представлено в ноутбуке DQN_discrete_BEST. Использовался алгоритм double DQN с отдельной target сетью и polyak averaging, также применялся reward shaping.

Для задачи MountainCarContinuous-v0 с континуальным action space лучшее решение представлено в ноутбуке REINFORCE_continuous_2_best. Использовался алгоритм REINFORCE или же Monte-Carlo policy gradient с reward shaping и стандартизацией состояний (sklearn.StandardScaler). Policy сеть выдает параметры нормального распределения, из которого сэмплятся actions. 
