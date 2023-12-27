unit Unit1;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, StdCtrls;

type
  TForm1 = class(TForm)
    Numbers: TMemo;
    Label1: TLabel;
    Ecount: TEdit;
    Label2: TLabel;
    Eres: TEdit;
    Label3: TLabel;
    Button1: TButton;
    Button2: TButton;
    procedure Button1Click(Sender: TObject);
    procedure Button2Click(Sender: TObject);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.dfm}

procedure TForm1.Button1Click(Sender: TObject);
Var i,summa, count: integer;
    rosa: longint;
    result:Real;
begin
 summa:=0;
 result:=0;
 count:= Numbers.Lines.Count;
 for i:=0 to count -1 do
  begin
   if not TryStrToInt(Numbers.Lines[i],rosa) then
     begin
      Numbers.Lines[i]:= 'Invalid';
      count:= count - 1;
      continue;
     end;

   summa:=summa+ rosa;
  end;

  result:= summa / count;
  Ecount.Text:= inttostr(count);
  Eres.Text:= floattostr(result);

end;

procedure TForm1.Button2Click(Sender: TObject);
begin
 Form1.Close;
end;

end.

