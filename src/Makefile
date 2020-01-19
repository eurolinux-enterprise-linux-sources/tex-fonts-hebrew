TEXMFDIR=/usr/share/texmf
CULMUSDIR=/usr/share/fonts/hebrew

tfms:
	./mkCLMtfm.sh

install:
	mkdir -p $(TEXMFDIR)/dvips/culmus/ \
		$(TEXMFDIR)/fonts/afm/public/ \
		$(TEXMFDIR)/fonts/type1/public/ \
		$(TEXMFDIR)/fonts/enc/dvips/culmus/ \
		$(TEXMFDIR)/fonts/map/dvips/ \
		$(TEXMFDIR)/fonts/tfm/public/culmus/ \
		$(TEXMFDIR)/fonts/vf/public/culmus/ \
		$(TEXMFDIR)/tex/latex/culmus/ \
		$(TEXMFDIR)/tex/generic/0babel/
	ln -s $(CULMUSDIR) $(TEXMFDIR)/fonts/afm/public/culmus
	ln -s $(CULMUSDIR) $(TEXMFDIR)/fonts/type1/public/culmus
	cp -p he8.enc $(TEXMFDIR)/fonts/enc/dvips/culmus/he8.enc
	cp -p culmus.map $(TEXMFDIR)/fonts/map/dvips/culmus.map
	cp -p *.tfm $(TEXMFDIR)/fonts/tfm/public/culmus/
	cp -p *.vf  $(TEXMFDIR)/fonts/vf/public/culmus/
	cp -p culmus.sty $(TEXMFDIR)/tex/latex/culmus/
	cp -p hebrew.ldf $(TEXMFDIR)/tex/generic/0babel/
#	cp -p he8enc.def he8frank.fd he8nachlieli.fd $(TEXMFDIR)/tex/latex/culmus/

clean:
	rm *.tfm *.vf *.vpl culmus.map
