deploy:
	git checkout source
	jekyll build
	git add -A
	git commit -m "update source"
	cp -r _site/ ~/tmp/_site/
	git checkout master
	rm -r ./*
	mkdir _site
	cp -r ~/tmp/_site/* _site/
	git add -A
	git commit -m "deploy update"
	git push origin master
	
	git checkout source
	echo "deploy succeed"
	git push origin source
	echo "push source"
