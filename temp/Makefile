run:
	dotnet run

build:
	dotnet build

publish:
	dotnet publish -r linux-musl-x64 --output "..\linux64_musl" --self-contained true -p:PublishSingleFile=true -p:PublishTrimmed=true
	fly deploy
	notify-send "Deployed to Fly.io"
