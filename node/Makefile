#Make install windows
# choco install make
run:
	docker run -d --nev-file ./config/.env --rm --name logsapp logsapp:env
stop:
	docker stop logsapp