# OOPs
package OOPs;

public class Student {
	String name;
	int rollNo;
	int marks;
	
	Student(String name,int rollNo,int marks){
		this.name=name;
		this.rollNo=rollNo;
		this.marks=marks;
	}
	String getGrade() {
		if(marks>=90) return "A";
		else if(marks>75 && marks<89) return "B";
		else if(marks>60 && marks<74) return "C";
		else return "D";
	}
	public static void main(String[] args) {
		Student s1=new Student("Ritika",101,99);
		Student s2=new Student("Ashu",102,85);
		Student s3=new Student("Pallavi",103,30);
		
		Student[] st = {s1,s2,s3};
		
		for(Student s : st) {
		System.out.println("Name : "+s.name + ", Roll No. : "+s.rollNo+ ", Marks : "+s.marks+", Grade : "+ s.getGrade());
		}
	}
}
