fun printIsoscelesTriangle(height: Int) {
    for (i in 1..height) {
        // Print spaces
        for (j in 1..(height - i)) {
            print(" ")  // This centers the stars for each row
        }
        // Print stars
        for (k in 1..(2 * i - 1)) {
            print("*")  // This prints stars in increasing odd numbers
        }
        println()  // Move to the next line after each row
    }
}

fun main() {
    val height = 5  // Set the height of the isosceles triangle
    printIsoscelesTriangle(height)  // Call the function to print the isosceles triangle
}
