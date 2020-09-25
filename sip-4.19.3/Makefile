
all:
	@(cd sipgen; $(MAKE))
	@(cd siplib; $(MAKE))

install:
	@(cd sipgen; $(MAKE) install)
	@(cd siplib; $(MAKE) install)
	@test -d $(DESTDIR)/home/liruiw/anaconda2/envs/omg_2/lib/python3.6/site-packages || mkdir -p $(DESTDIR)/home/liruiw/anaconda2/envs/omg_2/lib/python3.6/site-packages
	cp -f sipconfig.py $(DESTDIR)/home/liruiw/anaconda2/envs/omg_2/lib/python3.6/site-packages/sipconfig.py
	cp -f /home/liruiw/Downloads/orocos_kinematics_dynamics/sip-4.19.3/sipdistutils.py $(DESTDIR)/home/liruiw/anaconda2/envs/omg_2/lib/python3.6/site-packages/sipdistutils.py

clean:
	@(cd sipgen; $(MAKE) clean)
	@(cd siplib; $(MAKE) clean)
