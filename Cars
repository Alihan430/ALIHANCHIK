class Car:
    def __init__(self, brand, model, year, fuel=0):
        self.brand = brand
        self.model = model
        self.year = year
        self.fuel = fuel
        self.engine_on = False

    def start_engine(self):
        if self.fuel > 0:
            self.engine_on = True
            print("Двигатель запущен.")
        else:
            print("Нет топлива!")

    def stop_engine(self):
        self.engine_on = False
        print("Двигатель остановлен.")

    def refuel(self, liters):
        self.fuel += liters
        print(f"Заправлено {liters} л. Топливо: {self.fuel} л.")

    def drive(self, km):
        if not self.engine_on:
            print("Сначала запустите двигатель.")
            return

        fuel_needed = km * 0.1
        if self.fuel >= fuel_needed:
            self.fuel -= fuel_needed
            print(f"Проехали {km} км. Осталось топлива: {self.fuel:.1f} л.")
        else:
            print("Недостаточно топлива.")

# Пример использования
car = Car("Toyota", "Camry", 2020)
car.refuel(20)
car.start_engine()
car.drive(50)
car.stop_engine()
