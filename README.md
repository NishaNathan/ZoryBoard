# ZoryBoard
#PyrmaidInAlphabet in C# class Program

{ 
    static void Main(string[] args) 
    { 
      char ch = 'A'; 
      int i, j, l, m; 
      for (i = 1; i <= 4; i++) 
      { 
        for (j = 4; j >= i; j--) 
          { 
            Console.Write(" "); 
          }
         for (l = 1; l <= i; l++) 
         { 
            Console.Write(ch++); ch--; 
         } 
         for (m = 1; m < i; m++) 
         { 
           Console.Write(--ch); 
           Console.Write("\n"); ch = 'A'; 
         } 
       }
    }
}


#Removing Duplicate String in c#

{ 
    static void dupstr(String str) 
    { 
      int i; 
      string givstr = string.Empty; 
      for (i = 0; i < str.Length;i++) 
        { 
          if(!givstr.Contains(str[i])) 
            { givstr = givstr + str[i]; } 
        } 
       Console.WriteLine("Removed Duplicate String:" + givstr); 
     }

    static void Main(string[] args)
    {
        Console.WriteLine("Enter a string:");
        String orgstr = Console.ReadLine();
        dupstr(orgstr);
        Console.ReadLine();
    }
}
