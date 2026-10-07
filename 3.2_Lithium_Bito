class Hero:
    def __init__(self, name, hp):
        self.name = name
        self.__hp = hp  # Private attribute to protect hero's health data

    def take_damage(self, amount):
        """Safely reduce HP, ensuring it doesn't drop below 0."""
        self.__hp -= amount
        if self.__hp < 0:
            self.__hp = 0

    def get_hp(self):
        """Public method to safely read private __hp."""
        return self.__hp

    def __repr__(self):
        return f"Hero(Name: {self.name}, HP: {self.__hp})"


# --- Instantiate Heroes ---
arthur = Hero("Arthur", 100)
morgana = Hero("Morgana", 100)

# Arthur takes 10 damage
arthur.take_damage(10)

# --- Print HP Results ---
print(f"{arthur.name}'s HP: {arthur.get_hp()}")
print(f"{morgana.name}'s HP: {morgana.get_hp()}")
