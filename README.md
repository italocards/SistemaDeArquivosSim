► SIMULADOR DE SISTEMA DE ARQUIVOS COM JOURNALING

- Linguagem: Java 17
- Autores: João Italo Cardoso Lima, Daniel Alves Façanha
- Repositório: https://github.com/italocards/SistemaDeArquivosSim

► OBJETIVO
Simular operações de um sistema de arquivos com:
- Criação/remoção de arquivos e diretórios
- Journaling para recuperação de falhas
- Comandos avançados em subdiretórios

► COMANDOS IMPLEMENTADOS
---------------------------------
listar                Lista conteúdo do diretório raiz
listar_diretorio <dir> Lista conteúdo de subdiretório
criar_diretorio <nome> Cria novo diretório
criar_arquivo <nome>  Cria arquivo no diretório atual
criar_arquivo_em <dir> <arquivo> Cria arquivo em subdiretório
renomear_arquivo <antigo> <novo> Renomeia arquivo
copiar_arquivo <origem> <destino> Copia arquivo
mostrar_journal       Exibe log de operações
ajuda                 Mostra esta lista

► COMO EXECUTAR
---------------------------------
1. Compile o projeto:
   javac SimulatedFileSystem.java

2. Execute:
   java SimulatedFileSystem

3. Digite comandos no prompt:
   Ex: criar_diretorio documentos
       criar_arquivo_em documentos relatorio.txt

► ESTRUTURA DE ARQUIVOS
---------------------------------
- SimulatedFileSystem.java  (Classe principal)
- SimDirectory.java        (Representa diretórios)
- SimFile.java             (Representa arquivos)
- Journal.java             (Registra operações)
- base.dat                 (Dados serializados - NÃO EDITAR MANUALMENTE)

► IMPORTANTE
---------------------------------
- O arquivo base.dat armazena o estado do sistema (serializado)
- Não edite manualmente para evitar corrupção de dados
