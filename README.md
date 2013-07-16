Word Count
======



class word{

        public static void main(String args[])
        {
            BufferedReader br=new BufferedReader(InputStreamReader(Syatem.in));
            int line=0,word1=0,flag=0;
            char ch;
            ch=getChar();
            while(ch!=br.eof)
            {
                if(ch=='\n')
                {   line++;
                }
                if(ch==' '||ch=='\t')
                {   flag=0;
                }
                else if(flag==0)
                {
                    word1++;
                    flag=1;
                }
            }
            System.out.println(line+" "word1);
        }
}
