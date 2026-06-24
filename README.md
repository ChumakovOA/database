[//]: # (Начало блока с заданием)
**Задание 1: Питон ебучий**
<img width="1018" height="600" alt="image" src="https://github.com/user-attachments/assets/012f8eac-fb2e-4ecc-bdf3-46c70202256a" />

<details>
<summary><strong></strong></summary>

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
