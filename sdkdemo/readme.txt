��һ������������Զ���ؼ�ʹ�ã���ر�֤��������ȫһ�¡�
�ڶ���������Ӧ��quc.dll��libquc.a ���� quc.lib(MSVC����������)���ɵ���Ŀ�С�
��������ʹ�õ��ĸ��ؼ���ֻ��Ҫ����Ӧ�ؼ���ͷ�ļ����ɵ���Ŀ�м��ɡ����ɷ����ǽ���ͷ�ļ����Ƶ�sdkĿ¼����Ϊpro�ļ�д���Ǵ�sdkĿ¼��ȡͷ�ļ�����Ҳ�����Լ�����Ŀ¼��
���Ĳ�����Ŀ��pro�ļ��������
INCLUDEPATH += $$PWD/sdk

CONFIG(release, debug|release){
LIBS        += -L$$PWD/sdk/ -lquc
} else {
unix {LIBS  += -L$$PWD/sdk/ -lquc}
else {LIBS  += -L$$PWD/sdk/ -lqucd}
}

˵������sdkdemo�µ�dll��mingw 64λ+Qt5.12.3�汾�ġ��������滻���Լ�����������������ļ��������ļ���Ҫ�滻��msvc��������dll+lib��mingw��������dll+a��gcc��������so��clang��������dylib����ؼǵ�debug����debug�ģ�release����release�ģ����ܽ����ã�����debug���������dll�ŵ�release���ã������򲻿��Եġ�