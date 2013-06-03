deck-final-
===========
import java.util.ArrayList;

/**
 * Write a description of class Deck here.
 * 
 * @author (your name) 
 * @version (a version number or a date)
 */
public class Deck 
{
   

private String [] val  = {"ACE", "KING", "QUEEN", "JACK", "TEN", "NINE", "EIGHT", "SEVEN", "SIX", "FIVE", "FOUR", "THREE", "TWO"};
public static int values = 13; 
public static int suits = 4; 
public static int aCard =values * suits; 
Card[] allArray = new Card[52];



public Deck()
 {
     int i = 0;
     
{ 

    for(int y = 1; y <= suits; y++)
        {
          Card x = new Card(val[y],"HEARTS"); 
        i++; 
        }
    for(int j = 1; j <= suits; j++)
    {
        Card w = new Card(val[j], "SPADES");
        i++;
    }
    for(int u = 0; u <= suits; u++)
    {
        Card t = new Card(val[u], "DIAMONDS");
        i++;
    }
    for(int q = 0; q <= suits; q++)
    {
      Card b = new Card(val[q], "CLUBS");
        i++;
    }
    
}

}

 public void shuffle()
{
Card[] allArray = new Card[52];

    Random o = new Random();
    for (int k = topOfDeck; k >= 0; k--) 
    {
        int index = o.nextInt(k + 1);
        allArray[k] = cards[index];
     Card carCard = cards[k];
        card[k] = cards[index];
        card[index] = carCard;
    }
    // at this point, tempArray has all the cards selected in random order
    card = allArray;
}
}
