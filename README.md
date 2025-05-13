# projeto-flavio-a3
projeto de sistema de gerenciamento de arquivos
package provas;
import java.awt.Menu;
import java.io.File;
import java.io.IOException;
import java.nio.file.Files;
import java.nio.file.Path;
import java.nio.file.Paths;
import java.nio.file.StandardCopyOption;
import java.util.Scanner;
import java.io.FileWriter;
import java.io.PrintWriter;

public class Flavio {

	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		//Mostrar o menu
		
		
		
		System.out.println("MENU");
		System.out.println("[1] Abrir o arquivo");
		System.out.println("[2] Renomear arquivo");
		System.out.println("[3] Mover arquivo ");
		System.out.println("[4] Copiar arquivo");
		System.out.println("[5] Excluir arquivo");
		System.out.println("[6] Sair");
		
		receber();
	}

	
	private static int receber() {
		// recebe informacoes do usuario
		Scanner scanner = new Scanner(System.in);
		System.out.println("Escolha a opcao:");
		return scanner.nextInt();
		
	}
	
    public void salvarAcao(String acao) throws IOException{
    	try (PrintWriter writer = new PrintWriter(new FileWriter("log.txt", true))){
    		writer.println(acao);
    	} catch (IOException e) {
    		System.out.println("Error ao salvar acao no log");
    	}
    	
    		class Main{
    		public static void main (String[] args) {
    			Menu menu = new Menu();
    			FileManager fileManager = new FileManager();
    			Log log = new Log();
    			
    			public void exibirMenu() {
    				
    			}
    			
    			while (true) {
    				menu.exibirMenu();
    				int opcao = menu.receberOpcao();
    				
    				switch (opcao) {
    				case 1:
    					
    				}
    			}
    		
    		}
    	}
    }
}
    
