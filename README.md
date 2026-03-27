# Undergrde-years
This is my first GitHub repository.
# First Semester University Life Simulator
import random

def simulate_semester():
    # 1. Setting up the environment (The "World")
    semester_data = {
        "university": "Shivaji College",
        "season": "Winter/Spring Transition",
        "avg_temperature": 22,  # in Celsius
        "subjects": ["Physics", "Mathematics", "Programming Fundamentals", "English"],
        "status": "Active"
    }

    print(f"--- Welcome to First Semester at {semester_data['university']} ---")
    print(f"Current Weather: {semester_data['avg_temperature']}°C. Perfect for campus life.\n")

    # 2. The Academic Cycle (Using a List of Events)
    events = [
        "Orientation & Society Sign-ups",
        "Weekly Quizzes (The Struggle Begins)",
        "Mid-Term Exams week",
        "Sports Day & Cultural Fest",
        "Final Project Submissions",
        "Final Exams (The Grand Finale)"
    ]

    # 3. Simulating the Life Flow
    for week, event in enumerate(events, 1):
        print(f"Week {week}: {event}")
        
        # Adding some logic for specific events
        if "Quizzes" in event:
            score = random.randint(70, 95)
            print(f"   > Result: You scored {score}% in your Programming Quiz!")
        
        elif "Mid-Term" in event:
            print("   > Life Status: Late nights, heavy coffee, and library sessions.")
        
        elif "Sports Day" in event:
            temp_rise = semester_data['avg_temperature'] + 5
            print(f"   > Activity: Out on the field! It's {temp_rise}°C today.")
            print("   > Victory: You participated in the relay race!")
            
        elif "Final Exams" in event:
            print("   > Result: All subjects cleared! Time for semester break.")

    print("\n--- Semester 1 Complete! ---")

if __name__ == "__main__":
    simulate_semester()
