TableGenerateCmd �����
Usage: TableGenerateCmd -i ȯ�漳������ -c ������ -s �ҽ����� -l ���[kr|cn] -v ���Ͻ������ 
Option: -i ȯ�� ���� ���� ��
           �ݵ�� ���� ���ϰ� ���� ��ġ�� �־�� �Ѵ�.
           ������ ���� ���, TableGenerateCmd.ini ������ �о� �´�.
        -c ���� ���, ��ɾ�� ��ҹ��ڸ� �������� �ʴ´�. �ɼ��� �������� ������ [all]�� ����ȴ�.
           all: ��� ������ ���Ϸ� �����Ѵ�.
           idl: .IDL, .H, .CPP ���� �������� �����Ѵ�.
           c#: .CS ������ ���Ϸ� ����
           table: .TBL ������ ���Ϸ� ����
           string: .KOR�� ���� �������� ����
           db: .SQL�� ���� �������� ����
        -s �ҽ� ����. Excel������ ����Ǿ� �ִ� ��ġ ����
        -l ��� [kr|cn]
           kr: �ѱ���
           cn: �߱���
        -v ���� ����

examlpe:
    TableGenerateCmd.exe
		: �⺻ �ɼ��� ����Ͽ� ���α׷��� ������.
	TableGenerateCmd.exe -i TableGenerateCmd2.ini
		: TableGenerateCmd2.ini ���� ������ �о ���α׷��� ������
	TableGenerateCmd -c idl c# table
		: idl, c#, table ������ ���ϸ� ����
	TableGenerateCmd -i TableGenerateCmd2.ini -c string db
		: ȯ�� ���� ������ �о�� string, db ������ ������� ������.

Usage: TableGenerateCmd -s SourcePath(*.xls) -v ���Ͻ������ -l [kr|cn]
      => �ҽ� ���� ������ �Է��� ���,  $Version ��ũ�θ� ����� �� ����.
      ex) TableGenerateCmd -s D:\Temp\Table$Version

Usage: TableGenerateCmd -s Table_M12 -l cn -v M12 -c
