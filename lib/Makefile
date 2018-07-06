#
# Makefile for misc library.
#
ROOT=..
PLATFORM=$(shell $(ROOT)/systype.sh)
include $(ROOT)/Make.defines.$(PLATFORM)

LIBMISC	= libunp.a
LIB_OBJS =  connect_nonb.o connect_timeo.o daemon_inetd.o daemon_init.o dg_cli.o dg_echo.o error.o get_ifi_info.o gf_time.o host_serv.o family_to_level.o mcast_leave.o mcast_join.o mcast_get_if.o mcast_get_loop.o mcast_get_ttl.o mcast_set_if.o mcast_set_loop.o mcast_set_ttl.o my_addrs.o read_fd.o readline.o readn.o readable_timeo.o rtt.o signal.o signal_intr.o sock_bind_wild.o sock_cmp_addr.o sock_cmp_port.o sock_ntop.o sock_ntop_host.o sock_get_port.o sock_set_addr.o sock_set_port.o sock_set_wild.o sockfd_to_family.o str_cli.o str_echo.o tcp_connect.o tcp_listen.o tv_sub.o udp_client.o udp_connect.o udp_server.o wraplib.o wrapsock.o wrapstdio.o wrappthread.o wrapunix.o write_fd.o writen.o writable_timeo.o

all:	$(LIBMISC)

$(LIBMISC):	$(LIB_OBJS)
	$(AR) rv $(LIBMISC) $?
	$(RANLIB) $(LIBMISC)


clean:
	rm -f *.o a.out core temp.* $(LIBMISC)

