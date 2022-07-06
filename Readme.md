## 7.5. Основы golang
# Задача 1

    package main

    import (
        "fmt"
        "os"
    )

    func main() {
        fmt.Print("Enter a number: ")
        var metr float64
        fmt.Scan(os.Stdin, &metr)
        output := metr * 0.3048
        fmt.Println(output)
    }
Вывод</br>
Задаём 100 метров

    Enter a number: 30.48

    Program exited.
# Задача 2

    package main

    import "fmt"

    func main() {
        x := []int{48, -96, 86, 68, 7, 82, 63, 70, 4, -17, 83, 27, 19, 97, 9, 17}
        a := x[1]
        for i := 0; i < len(x); i++ {
            if x[i] < a {
                a = x[i]
            }
        }
        fmt.Println(a)
    }
Вывод для данной последовательности

    -96

    Program exited.
# Задача 3

        package main

        import "fmt"

        func main() {
            x := []int{}
            for i := 1; i < 101; i++ {
                if i%3 == 0 {
                    x = append(x, i)
                }
            }
            fmt.Println(x)
        }
Вывод
[3 6 9 12 15 18 21 24 27 30 33 36 39 42 45 48 51 54 57 60 63 66 69 72 75 78 81 84 87 90 93 96 99]

Program exited.