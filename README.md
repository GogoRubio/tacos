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
