# Q1

fun main() {
    // Step 1: Get input from the user
    println("Enter a weekday:")
    val weekday = readLine() ?: "" // Reading input from the user

    // Step 2: Print the weekday
    println("On $weekday, the opening hours are:")

    // Step 3: Use if-else-if to print opening hours
    if (weekday == "Monday") {
        println("9 AM to 5 PM (9:00 – 17:00)")
    } else if (weekday == "Tuesday") {
        println("9 AM to 5 PM (9:00 – 17:00)")
    } else if (weekday == "Wednesday") {
        println("9 AM to 5 PM (9:00 – 17:00)")
    } else if (weekday == "Thursday") {
        println("8 AM to 6 PM (8:00 – 18:00)")
    } else if (weekday == "Friday") {
        println("8 AM to 6 PM (8:00 – 18:00)")
    } else if (weekday == "Saturday") {
        println("10 AM to 4 PM (10:00 – 16:00)")
    } else if (weekday == "Sunday") {
        println("Closed")
    } else {
        println("Invalid day")
    }

    // Alternative Step 3: Using when statement
    when (weekday) {
        "Monday", "Tuesday", "Wednesday" -> println("9 AM to 5 PM (9:00 – 17:00)")
        "Thursday", "Friday" -> println("8 AM to 6 PM (8:00 – 18:00)")
        "Saturday" -> println("10 AM to 4 PM (10:00 – 16:00)")
        "Sunday" -> println("Closed")
        else -> println("Invalid day")
    }
}
