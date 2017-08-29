# Laboratorio Número 1
## ¿Qué es Github?
Github es una Plataforma que nos permite realizar repositorios de nuestro software  para que otras personas puedan visualizarlas y dar su opinión
## Qué es EclipseChe? 
Es una herramienta multiplataforma que se basa en la nube para que los desarrolladores puedan trabajar de manera local o remota.
## ¿Qué diferencia hay entre agragación y herencia?
La diferencia es que en agregación es una relación que define que un objeto es parte de otro objeto y Herencia se define como una clase creada por otra clases ya existente el cual puede contener atributos y métodos de la clase ya existente.
## ¿Que relación existe entre herencia y polimorfismo?
La relación que existe entre herencia y polimorfismo es que se pueden utiliazar sinteticamente objetos iguales a objetos de tipo distintos. 
### Instalar Eclipse Oxygen



1° Se debe descargar el ejecutable de la pagina: Eclipse.org


2° Se ejecuta el ejecutable y se instala.


3° Se prueba el programa. 

El nombre del ejecutable es: eclipse-inst-win64


# Documentación:

## a) Agregación:

### Clase:  Point 



	public class Line {
     private int X;
	  private int Y;
		
		public void Point() {
			
		}
		public void Point  (int X, int Y) {
			this.X = X;
			this.Y = Y; 
		}
		public int getx() {
			return X; 
		}
		public int gety() {
			return Y;
		}
		public void setx (int X) {
			this.X = X;
		}
		public void sety (int Y) {
			this.Y = Y;
		}
		public int []getxy (){
			int [] response = new int [2];
			response [0] = this.X;
			response [1] = this.Y;
			return response; 			
		}
		public void setxy(int X, int Y) {
			this.X = X;
			this.Y = Y;
			
		}
		
		public double Distance1 (double X2, double Y2) {
			double Distance1 = (double)Math.sqrt((Math.pow((X2-X), 2)+ Math.pow((Y2-Y), 2)));
			return Distance1;
					
		}
		public double Distance(double Distance1) {
			return Distance1; 
		}
	}
		

}




### Clase: Line




public class Line {
	
	Point PointDistance;
	private int X1;
	private int X2;
	private int Y1;
	private int Y2;
	
	
	
	
	public Line (int X1, int Y1, int X2, int Y2 ) {
		this.X1 = X1;
		this.Y1 = Y1;
		this.X2 = X2;
		this.Y2 = Y2; 
	}
	public Line( Point Begin, Point End) {
		
	}
	public Point getBegin() {
		return getBegin(); 
	}
	public void setBegin(Point Begin) {
		this.setBegin(Begin);
	}
	public Point getEnd() {
		return getEnd(); 
	}
	public void setEnd(Point End) {
		this.setEnd(End);
	}
	public int getBeginX() {
		return X1;
		
	}
	public void setBeginX(int X) {
		
	}
	public int getBeginY() {
		return Y1; 
	}
	public void setBeginY(int Y) {
		
	}
	public int[2] getBeginXY(){
		
	}
	public void SetBeginXY(int X, int Y) {
		
	}
	public int getEndX() {
		
	}
	public void getEndX(int X) {
		
	}
	public int getEndY() {
		
	}
	public void setEndY(int Y) {
		
	}
	public int[] getEndXY() {
		
	}
	public void setEndXY(int X, int Y) {
		
	}	
	
}


## b) Herencia:

### Clase: Person





  public class Person {
	public String Name;
	public String Address;
	
	public Person(String Name, String Address) {
		
	}
	public String getName() {
		return Name;
		
	}
	public String getAddress()
	{
		return Address;
	}
	
	public void setAddress(String Address) {
		
	}	
	public String ToString() {
		return Address; 
	}
	

}



### Clase: Student



public class Student extends Person {
	private int NumCourses = 0;
	private String[] Courses = {};
	private int [] Grades = {}; 
	
	public Student (String Name, String Address) {	
		super(Name, Address);
	}
	public String ToString() {
		return (super.getName() + " , " + super.getAddress() + " , " + NumCourses + "  ,  " + Courses+ "  ,   " + Grades);
	}
	public void  addCoursesGrade(String Course, int grade) {
		for(int i = 0; i <= Courses.length; i++) {
			if(Courses[i] != null) {
				Courses[i] = Course;
			}
			for(int j = 0; j <= Grades.length; j++) {
				if(Grades[i] != 0) {
					Grades[i] = grade;
				}
			}
		}
	}
	public void PrintGrades() {
		for(int i = 0; i<=Grades.length; i++) {
			if(Grades[i] != 0) {
				System.out.println(Grades[i]);
			}
		}
		
	}
	public double getAverageGrade() {
		return 0;	
	}
	public String ToString2() {
		return super.toString();
	}
	
	}
  
  
  
  ### Clase: Teacher
  
  
  
   public class Teacher {
   private	int NumCourses = 0;
   private String [] Courses = {};
	
	public Teacher (String Name, String Address) {
		
	}
	public boolean addCourses ( String Courses) {
		return false;
		
	}
	public boolean removeCoruses (String Courses) {
		return false;
		
	}
	
	}

