# - * - codificação: utf-8 - * -
from  tkinter  import  Tk , END , Entry , N , E , S , W , Button
da  fonte de importação do tkinter  
do  tkinter  import  Label
de  funções de  importação  parcial


def  get_input ( entrada , argumento ):
    entrada . inserir ( END , argumento )


def  backspace ( entrada ):
    input_len  =  len ( entrada . get ())
    entrada . delete ( input_len  -  1 )


def  claro ( entrada ):
    entrada . excluir ( 0 , END )


def  calc ( entrada ):
    input_info  =  entrada . obter ()
    tente :
        output  =  str ( eval ( input_info . strip ()))
    exceto  ZeroDivisionError :
        popupmsg ()
        output  =  ""
    limpar ( entrada )
    entrada . inserir ( END , saída )


def  popupmsg ():
    popup  =  Tk ()
    pop-up . redimensionável ( 0 , 0 )
    pop-up . geometria ( "120x100" )
    pop-up . título ( "Alerta" )
    label  =  Label ( popup , text = "Não é possível dividir por 0! \ n Insira valores válidos" )
    etiqueta . empacotar ( lado = "topo" , preencher = "x" , pady = 10 )
    B1  =  Botão ( pop-up , texto = "Ok" , bg = "#DDDDDD" , comando = pop-up . Destruir )
    B1 . pack ()


def  cal ():
    root  =  Tk ()
    root . título ( "Calc" )
    root . redimensionável ( 0 , 0 )

    entry_font  =  fonte . Fonte ( tamanho = 15 )
    entry  =  Entry ( root , justify = "right" , font = entry_font )
    entrada . grade ( linha = 0 , coluna = 0 , expansão da coluna = 4 ,
               pegajoso = N  +  W  +  S  +  E , padx = 5 , pady = 5 )

    cal_button_bg  =  '# FF6600 '
    num_button_bg  =  '# 4B4B4B'
    other_button_bg  =  '#DDDDDD'
    text_fg  =  '#FFFFFF'
    button_active_bg  =  '# C0C0C0'

    num_button  =  parcial ( botão , raiz , fg = text_fg , bg = num_button_bg ,
                         padx = 10 , pady = 3 , activebackground = button_active_bg )
    cal_button  =  parcial ( Botão , raiz , fg = text_fg , bg = cal_button_bg ,
                         padx = 10 , pady = 3 , activebackground = button_active_bg )

    button7  =  num_button ( text = '7' , bg = num_button_bg ,
                         command = lambda : get_input ( entrada , '7' ))
    button7 . grade ( linha = 2 , coluna = 0 , pady = 5 )

    button8  =  num_button ( text = '8' , command = lambda : get_input ( entrada , '8' ))
    button8 . grade ( linha = 2 , coluna = 1 , pady = 5 )

    button9  =  num_button ( text = '9' , command = lambda : get_input ( entrada , '9' ))
    button9 . grade ( linha = 2 , coluna = 2 , pady = 5 )

    button10  =  cal_button ( text = '+' , command = lambda : get_input ( entrada , '+' ))
    button10 . grade ( linha = 4 , coluna = 3 , pady = 5 )

    button4  =  num_button ( text = '4' , command = lambda : get_input ( entrada , '4' ))
    button4 . grade ( linha = 3 , coluna = 0 , pady = 5 )

    button5  =  num_button ( text = '5' , command = lambda : get_input ( entrada , '5' ))
    button5 . grade ( linha = 3 , coluna = 1 , pady = 5 )

    button6  =  num_button ( text = '6' , command = lambda : get_input ( entrada , '6' ))
    button6 . grade ( linha = 3 , coluna = 2 , pady = 5 )

    button11  =  cal_button ( text = '-' , command = lambda : get_input ( entrada , '-' ))
    button11 . grade ( linha = 3 , coluna = 3 , pady = 5 )

    button1  =  num_button ( text = '1' , command = lambda : get_input ( entrada , '1' ))
    button1 . grade ( linha = 4 , coluna = 0 , pady = 5 )

    button2  =  num_button ( text = '2' , command = lambda : get_input ( entrada , '2' ))
    button2 . grade ( linha = 4 , coluna = 1 , pady = 5 )

    button3  =  num_button ( text = '3' , command = lambda : get_input ( entrada , '3' ))
    button3 . grade ( linha = 4 , coluna = 2 , pady = 5 )

    button12  =  cal_button ( text = '*' , command = lambda : get_input ( entrada , '*' ))
    button12 . grade ( linha = 2 , coluna = 3 , pady = 5 )

    button0  =  num_button ( text = '0' , command = lambda : get_input ( entrada , '0' ))
    # button0.grid (linha = 5, coluna = 0, coluna = 2, padx = 3, pady = 5, aderente = N + S + E + W)
    button0 . grade ( linha = 5 , coluna = 0 ,   pady = 5 )

    button13  =  num_button ( text = '.' , command = lambda : get_input ( entrada , '.' ))
    button13 . grade ( linha = 5 , coluna = 1 , pady = 5 )

    button14  =  botão ( raiz , texto = '/' , fg = text_fg , BG = cal_button_bg , padx = 10 , pady = 3 ,
                      comando = lambda : get_input ( entrada , '/' ))
    button14 . grade ( linha = 1 , coluna = 3 , pady = 5 )

    button15  =  Botão ( raiz , texto = '<-' , bg = other_button_bg , padx = 10 , pady = 3 ,
                      command = lambda : backspace ( entrada ), activebackground = button_active_bg )
    button15 . grade ( linha = 1 , coluna = 0 , expansão da coluna = 2 ,
                  padx = 3 , pady = 5 , pegajoso = N  +  S  +  E  +  W )

    button16  =  Botão ( raiz , texto = 'C' , bg = other_button_bg , padx = 10 , pady = 3 ,
                      comando = lambda : limpar ( entrada ), fundo ativo = button_active_bg )
    button16 . grade ( linha = 1 , coluna = 2 , pady = 5 )

    button17  =  botão ( raiz , texto = '=' , fg = text_fg , BG = cal_button_bg , padx = 10 , pady = 3 ,
                      command = lambda : calc ( entrada ), activebackground = button_active_bg )
    button17 . grade ( linha = 5 , coluna = 3 , pady = 5 )

    button18  =  botão ( raiz , texto = '^' , fg = text_fg , BG = cal_button_bg , padx = 10 , pady = 3 ,
                      command = lambda : get_input ( entrada , '**' ))
    button18 . grade ( linha = 5 , coluna = 2 , pady = 5 )

    root . mainloop ()


if  __name__  ==  '__main__' :
    cal ()
