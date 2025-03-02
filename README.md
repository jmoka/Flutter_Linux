* INSTALANDO O JAVA

** JDK-17

		sudo apt install openjdk-17-jdk -y
	
** OUTRAS VERSÕES
*** LISTA AS VERSÕES DISPONÍVEIS

		sudo apt install openjdk-17-jdk -y
	
*** Configurar o Java no PATH
	
	- 	ABRA O ARQUIVO .BASHRC E COPIE OS ECHO
			
		source ~/.bashrc
	- OU ABRA EM PASTA PESSOAL O ARQUIVO OCULTO .BASHRC E COLE OS ECHO ABAIXO

		echo 'export JAVA_HOME="/usr/lib/jvm/java-17-openjdk-amd64"' >> ~/.bashrc
		echo 'export PATH=$JAVA_HOME/bin:$PATH' >> ~/.bashrc
	
* VERIFICAR O VERSÃO DO JAVA
	
		java -version


* INSTALAR O FLUTTER

** PACOTES(NECESSÁRIOS)
	
		sudo apt-get update -y && sudo apt-get upgrade -y;
		sudo apt-get install -y curl git unzip xz-utils zip libglu1-mesa

		sudo apt-get install libc6:amd64 libstdc++6:amd64 lib32z1 libbz2-1.0:amd64
	
** BAIXAR O PACOTE DO FLUTTER
	
		LINK DOWNLOADS :
		https://storage.googleapis.com/flutter_infra_release/releases/stable/linux/flutter_linux_3.29.0-stable.tar.xz

** DESCOMPACTANDO O PACOTE	
		
		- NA PASTA PESSOAL , CRIE UM PASTA CHAMADA DEVELOPMENT E DENTRO DELA COPIE A PASTA FLUTTER QUE ESTA DENTRO DO ARQUIVO BAIXADO, DESCOMPACTE E COLE DENTRO DE DEVELOPMENT

	
** Configurar o FLUTTER no PATH

** .bash_profile

	- NO CMD RODE O CODIGO:

			echo 'export PATH="$HOME/development/flutter/bin:$PATH"' >> ~/.bash_profile
			
	- OU ABRA O ARQUIVO .BASH_PROFILE QUE EST A DETRO DE PASTA PESSOAL,
	- ESTA OCULTO ABRA E COLE O CODIGO ABAIXO:
	
			export PATH="$HOME/development/flutter/bin:$PATH"
			
			
 ** .bashsc
 	
 	-ABRA O ARQUIVO E COPIE OS OS CAMINHSO ABAIXO
 	
 		export PATH="$HOME/development/flutter/bin:$PATH"
		export ANDROID_HOME=$HOME/Android/Sdk
		export ANDROID_SDK_ROOT=$HOME/Android/Sdk
		export PATH=$PATH:$HOME/Android/Sdk/cmdline-tools/latest/bin
		export PATH=$ANDROID_HOME/cmdline-tools/latest/bin:$ANDROID_HOME/platform-tools:$ANDROID_HOME/emulator:$PATH
		export JAVA_HOME="/usr/lib/jvm/java-11-openjdk-amd64"  # Certifique-se de que este caminho esteja correto
		export PATH=$JAVA_HOME/bin:$PATH

** .Zsh
 		
  		
  		echo 'export PATH="$HOME/development/flutter/bin:$PATH"' >> ~/.zshenv
			
	
** .Fish 
  

		fish_add_path -g -p ~/development/flutter/bin
			
** .Csh 
  
  		echo 'setenv PATH "$HOME/development/flutter/bin:$PATH"' >> ~/.cshrc
 

** .Tcsh
 
  		echo 'setenv PATH "$HOME/development/flutter/bin:$PATH"' >> ~/.tcshrc
 

** .profile
  
  		echo 'export PATH="$HOME/development/flutter/bin:$PATH"' >> ~/.profile


Após adicionar a linha correspondente ao seu shell, reinicie o terminal ou execute o seguinte comando para aplicar as alterações: 


		source ~/.bash_profile   
		source ~/.zshenv        
		source ~/.profile       

	
* Instalar Dependências do Flutter
	
	sudo apt install curl git unzip xz-utils zip libglu1-mesa -y

* Instalar o Android Studio e o SDK

	sudo snap install android-studio --classic

* Abrir o Android Studio e configurar o SDK

	android-studio

* Variaveis 
	
	echo 'export ANDROID_HOME=$HOME/Android/Sdk' >> ~/.bashrc
	echo 'export ANDROID_SDK_ROOT=$HOME/Android/Sdk' >> ~/.bashrc
	echo 'export PATH=$ANDROID_HOME/cmdline-tools/latest/bin:$ANDROID_HOME/platform-tools:$ANDROID_HOME/emulator:$PATH' >> ~/.bashrc


* Aceitar Licenças do Android SDK

	flutter doctor --android-licenses

* Instalar Ferramentas Necessárias para Desenvolvimento no Linux
	
	sudo apt install clang cmake ninja-build libgtk-3-dev -y

* Verificar Se Tudo Está Configurado
	
	flutter doctor	



* INSTALANDO O PRIMEIRO PROJETO FLUTTER
	
	flutter create meu_primeiro_app

	
* ANDROID STUDIO
	
	android-studio



			
