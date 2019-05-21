# Mountain_Car_Problem

Для задачи MountainCar-v0 с дискретным action space лучшее решение представлено в ноутбуке **DQN_discrete_BEST**. Использовался алгоритм double DQN с отдельной target сетью и polyak averaging, также применялся reward shaping.

Для задачи MountainCarContinuous-v0 с континуальным action space лучшее решение представлено в ноутбуке **REINFORCE_continuous_2_best**. Использовался алгоритм REINFORCE или же Monte-Carlo policy gradient с reward shaping и стандартизацией состояний (sklearn.StandardScaler). Policy сеть выдает параметры нормального распределения, из которого сэмплятся actions. 

Сети сохранял каждые 100 итераций, не всегда последняя сеть оказывалась лучшей, в ноутбуках смотрю как работают лучшая и последняя. Модели в виде state_dicts PyTorch лежат в папках models и cont_models, для дискретной и континуальной версий задачи соответсвенно.

Что еще пробовал:

Дискретизировал state space и попробовал табличный Q learning для задачи с дискретным action space, вагонетка научилась заезжать на холм, но больше чем за 200 итераций.
