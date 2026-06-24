[//]: # (Начало блока с заданием)
**Задание 1: Название задачи**

![Скриншот задания](<img width="820" height="951" alt="image" src="https://github.com/user-attachments/assets/500ff90a-24b1-47da-bfe4-dc7c106c6a1f" />
)

<details>
<summary><strong></strong> (нажмите, чтобы раскрыть)</summary>

```python
class Employee:
    def __init__(self, name, salary):
        self.name = name
        self.salary = salary

    def get_payout(self):
        return self.salary

class Manager(Employee):
    def __init__(self, name, salary, kpi_bonus):
        super().__init__(name, salary)
        self.kpi_bonus = kpi_bonus

    def get_payout(self):
        return self.salary + self.kpi_bonus

name = input().strip()
salary = float(input())
bonus = float(input())

m = Manager(name, salary, bonus)
print(f"К выплате менеджеру {m.name}: {m.get_payout()}")
```
</details>

[//]: # (Конец блока с заданием)
