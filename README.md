# Fundamentos da Internet e Protocolos

## Como a Internet Funciona

### Visão Geral
A internet é uma rede global que conecta milhões de dispositivos, permitindo comunicação e troca de dados através de uma infraestrutura complexa.

### Infraestrutura
- **Cabos e Roteadores:** Cabos submarinos e fios de fibra óptica conectam roteadores que transmitem dados.
- **Data Centers:** Armazenam e processam grandes volumes de dados.

### Transmissão de Dados
- **Pacotes:** Dados são divididos em pacotes pequenos e enviados por diferentes rotas.
- **Roteamento:** Roteadores direcionam os pacotes pela rede.

## HTTP/HTTPS

### Definição e Funcionamento
- **HTTP (Hypertext Transfer Protocol):** Protocolo que permite a comunicação na web para a transmissão de dados como páginas.
- **HTTPS (Hypertext Transfer Protocol Secure):** Versão segura do HTTP com criptografia para proteger os dados transmitidos.

### Diferenças entre HTTP e HTTPS
- **Segurança:** HTTPS utiliza SSL/TLS para criptografar a comunicação, enquanto HTTP não possui criptografia.

### Certificados SSL/TLS
- **SSL (Secure Sockets Layer):** Protocolo antigo que criptografa a comunicação entre o navegador e o servidor. Embora seja considerado obsoleto, o termo ainda é amplamente utilizado.
- **TLS (Transport Layer Security):** Sucessor do SSL, oferece criptografia e autenticação mais robustas. TLS garante a segurança na comunicação, protegendo dados contra espionagem e ataques.

### Métodos HTTP
- **GET:** Solicita dados de um servidor. 
  - Exemplo: Quando você visita `https://www.exemplo.com`, o navegador envia uma requisição GET para obter a página web.
- **POST:** Envia dados ao servidor para criar ou atualizar um recurso.
  - Exemplo: Ao preencher um formulário de registro e enviá-lo, o navegador usa POST para enviar os dados e criar uma nova conta de usuário.
- **PUT:** Substitui ou adiciona um recurso no servidor. Se o recurso não existir, é criado; se existir, é substituído.
  - Exemplo: Enviando uma requisição PUT para `https://api.exemplo.com/usuarios/123` com novos dados, o servidor atualiza ou cria o usuário com ID 123.
- **DELETE:** Remove um recurso do servidor.
  - Exemplo: Enviando uma requisição DELETE para `https://api.exemplo.com/usuarios/123`, o servidor remove o usuário com ID 123.
- **PATCH:** Faz alterações parciais em um recurso existente.
  - Exemplo: Enviando uma requisição PATCH para `https://api.exemplo.com/usuarios/123` para atualizar apenas o endereço de e-mail do usuário.

### Códigos de Status HTTP
- **200 OK:** Solicitação bem-sucedida.
- **404 Not Found:** Recurso não encontrado.
- **500 Internal Server Error:** Erro no servidor.

## Domínio

### Definição
Nome que identifica um site na web, facilitando a navegação. 
- Exemplo: `www.exemplo.com` é um nome de domínio que leva a um site específico.

## IP (Endereço IP)

### Definição
Identificador numérico único para cada dispositivo na rede. 
- Exemplo: Um endereço IP pode ser `192.168.1.1`, identificando um dispositivo específico.

## Host

### Definição
Computador ou servidor que armazena e fornece acesso a sites e serviços. 
- Exemplo: Um servidor web que hospeda um site é um host.

## DNS (Sistema de Nomes de Domínio)

### Definição
Sistema que traduz nomes de domínio em endereços IP. 
- Exemplo: O DNS converte `www.exemplo.com` em um endereço IP como `93.184.216.34` para que os navegadores possam encontrar o site.

## Cliente-Servidor

### Modelo Cliente-Servidor
Estrutura onde clientes solicitam serviços e servidores fornecem respostas.

### Exemplos
- **Navegação na Web:** Navegador (cliente) solicita páginas web; servidor envia as páginas.
- **E-mail:** Cliente de e-mail envia mensagens para um servidor de e-mail que entrega as mensagens.

## Redes e Topologias

### Redes
- **LAN (Rede Local):** Conecta dispositivos em uma área limitada.
- **WAN (Rede de Longa Distância):** Conecta redes em locais distantes.

### Topologias
- **Topologia em Estrela:** Dispositivos conectados a um ponto central.
- **Topologia em Malha:** Dispositivos interconectados, oferecendo múltiplos caminhos.

## Navegadores e Servidores Web

### Navegadores
Softwares que interpretam e exibem páginas web (Chrome, Firefox, etc.).

### Servidores Web
Programas que armazenam e fornecem páginas web para navegadores.

## Segurança na Internet

### Criptografia
Métodos de proteger dados através de codificação para segurança durante a transmissão.

### Proteção Contra Ataques
- **Phishing:** Engana usuários para obter informações pessoais.
- **Malware:** Software malicioso para causar danos ou roubar informações.
