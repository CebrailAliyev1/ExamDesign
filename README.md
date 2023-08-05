# ExamDesign
Sual 1
The ViewHolder is a wrapper around a View that contains the layout for an individual item in the list. The Adapter creates ViewHolder objects as needed and also
sets the data for those views. The process of associating views to their data is called binding.
Sual 2
We can use the try-catch block for exception handling in Kotlin.
val number = try {
    val message = "Welcome to Kotlin Tutorials"
    message.toInt()
} catch (exception: Exception) {
}
return number
Sual 3
Decorator pattern allows a user to add new functionality to an existing object without altering its structure. This type of design pattern comes under structural pattern as this pattern acts as a wrapper to existing class.
Sual 4
var array = listOf<Int>(1,2,1,3,4,2)
var temp = intArrayOf()
for (i in array)
{
    if (i in temp)
    {
        continue
    }else{
        temp += i
    }
}
for (j in temp)
{
    println("Element $j")
}
Sual 5
In Kotlin, let() is a pretty convenient scope function. It allows us to transform the given variable to a value in another type. In this tutorial, we'll explore how to apply let-like operations on multiple variables.
Sual6
solid prinsipi pozulmayib.
Sual 7
Companion object komeyi ile declare edirik kotlinde
Sual 8
A Kotlin constructor is a special member function in a class that is invoked when an object is instantiated.bir nece cur constructor var
parameterli parametrsiz,nested
eger moterize daxilinde varsa parametrli yoxsa parametrsiz
Sual 9
The factory design pattern says define an interface ( A java interface or an abstract class) for creating object and let the subclasses decide which class to instantiate. Factory Method Pattern allows the sub-classes to choose the type of objects to create.
Sual 10
enum class HouseFactory {
    Cottage,Villa
}
//bu Fabrikalarin hansi metodlari implement edilecek
interface AbstractFactory{
   fun buildercottage()
   fun buildCarVilla()
}

class AbstractFactoryProvider(){
    fun getFactory(factory: FactoryType):AbstractFactory{
      return  when(factory){
            FactoryType.Cottage-> CottageFactory()
            FactoryType.Villa-> VillaFactory()
        }
    }
}
class CottageFactory():AbstractFactory {
    override fun builderCottage() {
        //Build cottage
    }

    override fun buildType() {
        //Build  villa
    }

}

    class VillaFactory():AbstractFactory{
        override fun builderCottage() {
            //Build cottage
        }

        override fun buildType() {
            //Build villa
        }
}
fun main(){
    val abstractFactoryProvider=AbstractFactoryProvider()
    abstractFactoryProvider.getFactory(FactoryType.AUDI).buildCarType()
    abstractFactoryProvider.getFactory(FactoryType.BMW).buildCarType()
}
Sual 11
LiveData məlumat sahibi sinifdir. daimi müşahidə olunandan fərqli olaraq, LiveData is lifecycle-aware,, app components, fraqments və activities kimi digər proqram komponentlərinin həyat dövrünə baxir.
Sual 12

Sual 13
fun Product(arr: IntArray): Int {
    var enboyuk1 = arr[0]
    var enboyuk2 = arr[0]

    for (num in arr) {
        if (num > enboyuk1) {
            enboyuk2 = enboyuk1
            enboyuk1 = num
        } else if (num > enboyuk2) {
            enboyuk2 = num
        }
    }

    return enboyuk1 * enboyuk2
}

fun main() {
    val nums = intArrayOf(2, 3, 1, 5, 6, 4)
    val result = Product(nums)
    println("Maximum product of two integers: $result")
}


Sual 14
The Singleton Pattern is a software design pattern which ensures that a class has only one instance and provides a global point of access to the object of that class.
Sual 15
