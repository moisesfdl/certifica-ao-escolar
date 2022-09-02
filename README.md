# certifica-ao-escolar


#include <iostream>
#include <tchar.h>
#include <httpext.h>
#define direitoCursoSuperior = faculdade
#define faculdade = CienciaDaComputaçao
#define rh
#define _certificado2Grau

using namespace std;
int main(int argc, char** argv)
{
	_tsetlocale;
	GLOBALHANDLE('mec');
	//#body...mec
	int *ptr;
		int certificado2Grau = ('certificado :'); 
		int Escola = ('E.E.S.G JOAO CURSINO'); 
		int LeiAparatoLegal = ('de acordo com o artigo 16 da lei nº 5.692/71'); 
		int certificaA = ('Moises Ferreira de Lima');
		int rg = ('R.G.:27.950.938-8');
		int ConfirmandoConclusao = ('concluiu os estudos do 2º Grau , no ano letivo de 1997 estando apto ao prosseguimento dos estudos em curso de Nivel Superior'); 
		int MinisterioEscolar =  ('SECRETARIA DA ESCOLA ESTADUAL , reconhecilo pelo mec'); 
		int DataConclusao = ('data:14/02/1998');
		int AssinaturaAluno = ('Ass:Moises Ferreira De Lima');
		int AssinaturaSecretarioRegional = ('Secretario Regional ASS: Regina Celia de Azevedo RG:17.059.798');
		int AssinaturaDiretorRegional = ('Diretor Reg. ou R.G ASS: Setsuko Kotinda Yonashiro RG:5.168.2.18 ');
		int mec = ('http://portal.mec.gov.br/par/consultas');
		*ptr = certificaA;
		certificado2Grau = Escola+LeiAparatoLegal+certificaA+rg+ConfirmandoConclusao+MinisterioEscolar+DataConclusao+AssinaturaAluno+AssinaturaSecretarioRegional+AssinaturaDiretorRegional;
		mec = certificado2Grau;
		cout << &mec << "\n"<<"Meu Certificado 2ª Grau: [" << &certificado2Grau<<"]"<< endl; 
	return 0;
}
