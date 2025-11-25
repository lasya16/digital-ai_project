# digital-ai_project hellooo 
 def movie_quiz_chatbot():
    print("🎬 Welcome to the Movie Quiz Chatbot!")
    print("Type 'quit' anytime to exit.\n")

    score = 0

    questions = [
        {"question": "1. Who is the main character in 'Iron Man'?", "answer": "tony stark"},
        {"question": "2. Which movie has the quote: 'May the Force be with you'?", "answer": "star wars"},
        {"question": "3. Who directed 'Inception'?", "answer": "christopher nolan"},
        {"question": "4. What is the highest-grossing film of all time?", "answer": "avatar"},
        {"question": "5. Which movie features the character 'Jack Sparrow'?", "answer": "pirates of the caribbean"},
        {"question": "6. Which superhero is known as the 'Dark Knight'?", "answer": "batman"},
        {"question": "7. Which movie won Best Picture at the Oscars in 2020?", "answer": "parasite"},
        {"question": "8. What is the name of the wizarding school in Harry Potter?", "answer": "hogwarts"},
        {"question": "9. Who played the Joker in 'The Dark Knight'?", "answer": "heath ledger"},
        {"question": "10. Which movie franchise features the Infinity Stones?", "answer": "marvel"}
    ]

    for q in questions:
        print(q["question"])
        user_answer = input("Your answer: ").lower().strip()

        if user_answer == "quit":
            print("Exiting quiz…")
            break

        if user_answer == q["answer"]:
            print("✔️ Correct!\n")
            score += 1
        else:
            print(f"❌ Wrong! Correct answer: {q['answer'].title()}\n")

    print(f"🎉 Quiz finished! Your score: {score}/{len(questions)}")


# Run the chatbot
movie_quiz_chatbot()
