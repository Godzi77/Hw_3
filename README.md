class TransportnyiZasib:
    def __init__(self, speed):
        self.speed = speed  # швидкість транспорту (км/год)

    def peremishchennia(self):
        print(f"Транспорт рухається зі швидкістю {self.speed} км/год.")

class Avtomobil(TransportnyiZasib):
    def __init__(self, speed, marka):
        super().__init__(speed)
        self.marka = marka

    def peremishchennia(self):
        print(f"Автомобіль {self.marka} їде зі швидкістю {self.speed} км/год.")

class Potiah(TransportnyiZasib):
    def __init__(self, speed, kilkist_vahoniv):
        super().__init__(speed)
        self.kilkist_vahoniv = kilkist_vahoniv

    def peremishchennia(self):
        print(f"Потяг із {self.kilkist_vahoniv} вагонами рухається зі швидкістю {self.speed} км/год.")

class Litak(TransportnyiZasib):
    def __init__(self, speed, vysota_polotu):
        super().__init__(speed)
        self.vysota_polotu = vysota_polotu

    def peremishchennia(self):
        print(f"Літак летить на висоті {self.vysota_polotu} м зі швидкістю {self.speed} км/год.")

if __name__ == "__main__":
    transport = TransportnyiZasib(60)
    auto = Avtomobil(120, "Toyota")
    potiah = Potiah(80, 12)
    litak = Litak(850, 10000)

    transport.peremishchennia()
    auto.peremishchennia()
    potiah.peremishchennia()
    litak.peremishchennia()


