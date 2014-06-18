
/**Class1 est la classe qui regroupe les methodes pour afficher remplir ou utiliser le tableau*/

import java.util.*;


public class Class1 {


	Scanner sc = new Scanner(System.in);

	/**parcourir et afficher tableau**/
	public void parcourirTableau(int[] tab)
	{
		for (int i=0; i< tab.length; i++){

			System.out.print(tab[i]+" "); }
		System.out.print("\n");	
	}


	/**remplir tableau avec ligne de commande*/
	public void remplirTableau(String [] argument,int[] tab)
	{


		for(int a=0; a<argument.length;a++)
		{
			tab[a]= Integer.parseInt(argument[a]);
//hiihh
		}

	}

	/**remplir tableau aleatoirement*/
	public void remplirTableauAleatoire (int[] tab)
	{

		for (int i=0; i< tab.length; i++){

			tab[i] = (int) (Math.random()*(20-0)+0);
		}

		parcourirTableau(tab);
	}


	/**trier tableau par ordre croissant*/

	public void trierTableau(int[] tab){

		/**have change sert a sortir de la boucle quand l'ordre croissant est realise*/
		boolean haveChange = true;
		while(haveChange){
			haveChange = false;
			for(int k=0; k<tab.length-1; k++){
				if(tab[k]>tab[k+1]){
					int temp = tab[k]  ;    
					tab[k] = tab[k+1];
					tab[k+1] = temp;
					haveChange = true;
				}
			}
		}


		parcourirTableau(tab);
	}

	/**trouver le min du tableau*/
	public int minTableau (int[]tab){  
		/**initialiser le minimum a la premiere valeur du tableau*/
		int minValue = tab[0];  
		for (int i=0; i< tab.length; i++){

			if(tab[i] < minValue){  
				minValue = tab[i];  
			}  

		}
		return minValue;  
	} 

	/**trouver le max du tableau*/
	public int maxTableau (int[] tab){  
		/**initialiser le maximum a la premiere valeur du tableau*/
		int maxValue = tab[0];  
		for (int i=0; i< tab.length; i++){

			if(tab[i] > maxValue){  
				maxValue = tab[i];  
			}  

		}
		return maxValue;
	} 

	/**trouver la moyenne du tableau*/
	public float moyTableau (int[] tab){  
		/**initialisation moyenne = 0 somme de toutes les valeurs = 0 et a (le nombre de chiffres) = 0 */
		float moyValue=0;
		int somme = 0;
		int a = 0;
		for (int i=0; i< tab.length; i++){

			somme += tab[i];
			a++;

		}
		moyValue = ((float)(somme)/(float)(a));
		return moyValue;
	}

	/**rechercher nombre dans un tableau*/
	public void rechercheTableau(int[] tab){
		/**a sert a indiquer si le chiffre se trouve dans le tableau et b represente l'emplacement de ce chiffre*/
		int a=0;
		int b=0;
		System.out.println("\nIndiquez le nombre que vous voulez chercher");
		/**Exception si la valeur entree par l'utilisateur n'est pas un entier*/
		try{
			/** Val est la valeur que l'utilisateur va entrer*/
			int val = sc.nextInt();

			for (int i=0; i< tab.length; i++){

				if (tab[i] == val)
				{
					b=i;
					a=1;	
				}

			}
			if (a==1) {System.out.println("\nle nombre "+val+" existe dans le tableau et a pour coordonn�es ("+b+")");
			System.out.println("\nSi vous voulez cherchez un autre nombre appuyez encore et r�esseyez");}
			else {System.out.println("\nle nombre "+val+" n'existe pas dans le tableau");	
			System.out.println("\nSi vous voulez cherchez un autre nombre appuyez encore et r�esseyez");}
		}
		catch (InputMismatchException e){
			System.out.print("\nLa valeur entr�e ne correspond pas � un entier\n Appuyez encore et r�esseyez");
			sc.nextLine();
		}//lol
	}




}



