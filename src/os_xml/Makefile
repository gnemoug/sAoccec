# Makefile for os_xml
# Daniel B. Cid <daniel.cid@gmail.com>||<daniel@underlinux.com.br>

PT = ../
NAME = os_xml

include ../Config.Make

SRCS =  os_xml.c os_xml_access.c os_xml_node_access.c os_xml_variables.c os_xml_writer.c
OBJS =  os_xml.o os_xml_access.o os_xml_node_access.o os_xml_variables.o os_xml_writer.o

xml:
		$(CC) -DXML_VAR=\"var\" $(CFLAGS) -c $(SRCS)
		ar cru os_xml.a ${OBJS}
		ranlib os_xml.a

clean:
		${CLEAN}
