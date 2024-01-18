class LoveSimulation:
    def __init__(self, attraction, compatibility, trust, communication):
        self.attraction = attraction
        self.compatibility = compatibility
        self.trust = trust
        self.communication = communication

    def update_attraction(self, new_attraction):
        self.attraction = new_attraction

    def update_compatibility(self, new_compatibility):
        self.compatibility = new_compatibility

    def update_trust(self, new_trust):
        self.trust = new_trust

    def update_communication(self, new_communication):
        self.communication = new_communication

    def evaluate_relationship(self):
        relationship_score = self.attraction + self.compatibility + self.trust + self.communication
        return relationship_score

# Example usage:
love_sim = LoveSimulation(8, 6, 4, 7)

# After a period of time, attraction and compatibility decrease.
love_sim.update_attraction(6)
love_sim.update_compatibility(4)

# Trust increases, communication also increases.
love_sim.update_trust(5)
love_sim.update_communication(8)

# Evaluate the relationship based on the updated factors.
print(f"The relationship score is: {love_sim.evaluate_relationship()}")
