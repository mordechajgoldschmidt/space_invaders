class Settings:
    """Klasa przeznaczona do przechowywania wszystkich ustawien gry."""

    def __init__(self):
        """Inicjalizacja danych statystycznych gry."""
        #Ustawienia ekranu
        self.screen_width = 1800
        self.screen_height = 900
        self.bg_color = (255, 255, 255)

        #Ustawienia dotyczace szybkosci statku
        self.ship_limit = 2

        #Ustawienia doytyczace pocisku
        self.bullet_width = 3
        self.bullet_height = 15
        self.bullet_color = (60, 60, 60)
        self.bullets_allowed = 5

        #UStawienia dotyczace obcego
        self.fleet_drop_speed = 15

        #Latwa zmiana szybkosci gry
        self.speedup_scale = 1.1

        #Latwa zmiana liczby punktow przyznawanych za zestrzelenie obcego
        self.score_scale = 1.5

        self.initialize_dynamic_settings()

    def initialize_dynamic_settings(self):
        """Inicjalizacja ustawien, ktore ulegaja zmianie w trakcie gry."""
        self.ship_speed = 4.5
        self.bullet_speed = 4.0
        self.alien_speed = 4.0

        #Wartosc fleet_direction wynoszaca 1 oznacza prawo, a -1 lewo
        self.fleet_direction = 1

        #Punktacja
        self.alien_points = 50

    def increase_speed(self):
        """Zmiana ustawien dotyczacych predkosci i liczby przyznawanych punktow."""
        self.ship_speed *= self.speedup_scale
        self.bullet_speed *= self.speedup_scale
        self.alien_speed *= self.speedup_scale

        self.alien_points = int(self.alien_points * self.score_scale)
