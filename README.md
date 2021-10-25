# Phantom



class Vehicle():
    def __init__(self, weight):
        print('Vehicle class created')
        self.weight = weight
        self.number_wheels = 4

    def _mytype(self):
        print('Type Vehicle')

vehicle = Vehicle(1000)
vehicle._mytype()

class Car(Vehicle):
    def __init__(self,weight):
        Vehicle.__init__(self, weight)
        print('\nCar class created')
        self.number_doors = 2

    def car_name(self):
        print('bugatti')

    def _mytype(self):
        print('Type Car')

car = Car(800)
car.car_name()
car._mytype()
print(car.number_wheels, car.number_doors)

class Terminator(Vehicle):
    def __init__(self,weight):
        Vehicle.__init__(self, weight)
        print('\nTerminator class created')
        self.number_doors = 0

    def robot_name(self):
        print('R2D2')

    def _mytype(self):
        print('Type Terminator')

Terminator = Terminator(10000)
Terminator.robot_name()
Terminator._mytype()
print(Terminator.number_wheels, Terminator.number_doors)

class ATV(Vehicle):
    def __init__(self,weight):
        Vehicle.__init__(self, weight)
        print('\nATV class created')
        self.number_doors = 0

    def atv_name(self):
        print('dude')

    def _mytype(self):
        print('Type ATV')

atv = ATV(100)
atv.atv_name()
atv._mytype()
print(atv.number_wheels, atv.number_doors)
