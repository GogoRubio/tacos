# tacos
public class Taco {
	
	private int Marisco;
	private int Canasta;
	private int Asadero;
	private double descuento;
	private double precio;
	
	
	public int getmarisco(){
		return Marisco; 
	}
	
	public void setmarisco(int setmarisco){
		this.Marisco=setmarisco;
		
	}
	
	public int getcanasta(){
		return Canasta;
	}
	
	public void setcanasta(int setcanasta){
		this.Canasta=setcanasta;
		
	}
	
	public int getasadero(){
		return Asadero;
	}
	
	public void setasadero(int setasadero){
		this.Asadero=setasadero;
		
	}
	
	public double descuento(double getdescuento){
		this.descuento=getdescuento;
		return descuento;
		
		
	}
	
	public double preciot(double setprecio){
		this.precio=setprecio;
		if (precio>10 && precio<20){
			return precio;
		}else {
			System.out.println("no es adecuado el precio");
		}
		
		precio=(setprecio-(setprecio*descuento));
		System.out.println("el precio del taco es:"+precio);
		return precio;
		
		
	}
	
	

}

public class Marisco extends Taco {
	private double precio;

	
	public double descuentomarisco(int setprecio){
		this.precio=setprecio;
		precio=setprecio-(setprecio*super.descuento(.12));
		return precio;
	}
		
		

}



public class Canasta extends Taco {
private double precio;

	
	public double descuentocanasta(int setprecio){
		this.precio=setprecio;
		precio=setprecio-(setprecio*super.descuento(.12));
		return precio;
	}
}



public class Asadero extends Taco {
private double precio;

	
	public double descuentoasadero(int setprecio){
		this.precio=setprecio;
		precio=setprecio-(setprecio*super.descuento(.12));
		return precio;
	}
}



public class app {

	public static void main(String[] args) {
	
		Marisco m=new Marisco();
		m.setmarisco(10);
		m.descuentomarisco(15);
		m.descuento(.12);
		
		
		
		Canasta c=new Canasta();
		c.setcanasta(10);
		c.descuentocanasta(18);
		c.descuento(.23);
		
		
		Asadero a=new Asadero();
		a.setasadero(10);
		a.descuentoasadero(17);
		a.descuento(.60);
		
		
		
		
