# proyecto-login

El scrip login.sql es para mysql : 
Requerimientos: 
genera un login con java se ,
 que ocupas un ide como el sprint tools suits , eclipse, netbean etc.
 
 java 
 
 1. clase main 

public static void main (String [] args) {

}
 2. clase de conexion a mysql 

impor java.sql.*;

public Connection con(){ 

class.forName("com.mysql.jdbc.Driver");
DriverManager.getConnection(URL_BASE_DE_DATOS,USUSARIO_PASSWORD);

}

public boolean buscarUsuarioBase(Sting usuario, String pass)
{ 
boolean login=false;
String sql= 
   Statement stm = this.con().createStatement();
   sql="SELECT * FROM login where usuario ="+usuario+" and  pass "+pass+"";
   Resultset rs= rs.sem.executeQuery(sql);
   if (rs.getString(2) !=null) {
     login=true; 
       }

 return login ; 
      

}


}
 3. clase que maneja el front 
