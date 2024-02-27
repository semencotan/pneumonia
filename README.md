# pneumonia
class Pneumonia:
    def __init__(self, symptoms, severity="Средняя"):
        self.symptoms = symptoms
        self.severity = severity

    def update_severity(self, new_severity):
        self.severity = new_severity

    def __str__(self):
        return f"Пневмония (Симптомы: {', '.join(self.symptoms)}, Степень тяжести: {self.severity})"

# Пример использования класса Pneumonia
pneumonia1 = Pneumonia(["Кашель", "Затрудненное дыхание"])
print(pneumonia1)

pneumonia1.update_severity("Тяжелая")
print(pneumonia1)
