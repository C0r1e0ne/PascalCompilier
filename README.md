# PascalCompilier
Компилятор Pascal на Python  

Команда:
- Ащеулов Дмитрий
- Токарев Даниил
- Давыдов Игорь
____
Входные данные:
```
Program beer;
            var
            e, b : integer;
            d, f: array [1 .. 100] of integer;

            function Alpha(a: integer):integer;
            var g: integer;
            begin
            a:=a*10;
            end;

            BEGIN
            e:=0;
            while (g<10) do
            begin
                d[1]:=g;
                Write(d[1]);
                g:=g+1;
            end;

            g:=Alpha(4);
            WriteLn(g);

            END.
```
____
Выходные данные:
```
Program
├ beer
├ var
│ ├ var_dec
│ │ ├ idents
│ │ │ ├ e
│ │ │ └ b
│ │ └ integer
│ ├ arr_decl
│ │ ├ integer
│ │ ├ idents
│ │ │ ├ d
│ │ │ └ f
│ │ ├ 1 (int)
│ │ └ 100 (int)
│ └ function
│   ├ Alpha
│   ├ params
│   │ └ var_dec
│   │   ├ idents
│   │   │ └ a
│   │   └ integer
│   ├ integer
│   ├ var
│   │ └ var_dec
│   │   ├ idents
│   │   │ └ g
│   │   └ integer
│   └ Body
│     └ ...
│       └ :=
│         ├ a
│         └ *
│           ├ a
│           └ 10 (int)
└ Body
  └ ...
    ├ :=
    │ ├ e
    │ └ 0 (int)
    ├ while
    │ ├ <
    │ │ ├ g
    │ │ └ 10 (int)
    │ └ ...
    │   ├ :=
    │   │ ├ d [1 (int)]
    │   │ └ g
    │   ├ call
    │   │ ├ Write
    │   │ └ d [1 (int)]
    │   └ :=
    │     ├ g
    │     └ +
    │       ├ g
    │       └ 1 (int)
    ├ :=
    │ ├ g
    │ └ call
    │   ├ Alpha
    │   └ 4 (int)
    └ call
      ├ WriteLn
      └ g
```
