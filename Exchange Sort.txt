package com.ck.learnings

fun main(){

    val exs = ExchangeSort()
    exs.exchangeSort()
}
class ExchangeSort {
    fun exchangeSort(){
        val num = intArrayOf(5,4,8,3,2,17)
        println("Array before sorting")
        for (i in num){
            print(" $i")
        }
        println()

        val num2 = intArrayOf(5,4,8,3,2,17)
        for (i in num.indices){
            for (j in i+1 until num.size){ // last index = 5
                if (num[i] > num[j]){   // num[0] > num[1}
                    var temp = num[j]
                    num[j]  = num[i]
                    num[i]  = temp
                }
                print(" i = $i , j = $j")
                println()
                for (item in num){
                    print(" $item")
                }
               println()
            }
            println()

        }
        println("Array before sorting")
        for (k in num){
            print(" $k")

        }
    }


}