����Dancer APP�����ַ���
1��
	���� dancer -a  myapp��
	��lib/myapp.pm ��ֱ�����ö�Ӧ·�ɣ�

	package Myweb;                                                                                                                                                  
	use Dancer ':syntax';

	our $VERSION = '0.1';

	get '/' => sub {
   		 template 'index';
	};
	
	...
	
	true;

2��	ֱ����һ���ű� myapp.pl
	
	#!/usr/bin/perl

	use Dancer;

	get '/' => sub{
        	return "HELLO WORLD!\n";
	};
	...
	start;