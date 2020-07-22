# DataBindingBasic-kotlin
Very Basic Example of Data Binding Android

Basic Example to show data binding basic to bind data with xml using data binding concept

data class Employee(
    var id: Int,
    var name: String,
    var email: String
)

 binding = DataBindingUtil.setContentView(this,R.layout.activity_main)
        binding.employee = getEmp()
        
        
 private fun getEmp(): Employee {
        return Employee(1,"John","jk@outlook,.com")
    }
