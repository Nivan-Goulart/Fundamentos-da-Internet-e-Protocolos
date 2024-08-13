<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fundamentos da Internet e Protocolos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        header {
            background: #333;
            color: #fff;
            padding-top: 30px;
            min-height: 70px;
            border-bottom: #ddd 3px solid;
            text-align: center;
        }
        header h1 {
            margin: 0;
        }
        section {
            background: #fff;
            padding: 20px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
        }
        h2 {
            color: #333;
        }
        ul {
            list-style-type: disc;
            margin-left: 20px;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Fundamentos da Internet e Protocolos</h1>
        </div>
    </header>
    <div class="container">
        <section>
            <h2>1. Como a Internet Funciona</h2>
            <p><strong>Visão Geral:</strong> A internet é uma rede global que conecta milhões de dispositivos, permitindo comunicação e troca de dados através de uma infraestrutura complexa.</p>
            <p><strong>Infraestrutura:</strong></p>
            <ul>
                <li><strong>Cabos e Roteadores:</strong> Cabos submarinos e fios de fibra óptica conectam roteadores que transmitem dados.</li>
                <li><strong>Data Centers:</strong> Armazenam e processam grandes volumes de dados.</li>
            </ul>
            <p><strong>Transmissão de Dados:</strong></p>
            <ul>
                <li><strong>Pacotes:</strong> Dados são divididos em pacotes pequenos e enviados por diferentes rotas.</li>
                <li><strong>Roteamento:</strong> Roteadores direcionam os pacotes pela rede.</li>
            </ul>
        </section>
        
        <section>
            <h2>2. HTTP/HTTPS</h2>
            <p><strong>Definição e Funcionamento:</strong></p>
            <ul>
                <li><strong>HTTP (Hypertext Transfer Protocol):</strong> Protocolo que permite a comunicação na web para a transmissão de dados como páginas.</li>
                <li><strong>HTTPS (Hypertext Transfer Protocol Secure):</strong> Versão segura do HTTP com criptografia para proteger os dados transmitidos.</li>
            </ul>
            <p><strong>Diferenças entre HTTP e HTTPS:</strong></p>
            <ul>
                <li><strong>Segurança:</strong> HTTPS utiliza SSL/TLS para criptografar a comunicação, enquanto HTTP não possui criptografia.</li>
            </ul>
            <p><strong>Certificados SSL/TLS:</strong></p>
            <ul>
                <li><strong>SSL (Secure Sockets Layer):</strong> Protocolo antigo que criptografa a comunicação entre o navegador e o servidor. Embora seja considerado obsoleto, o termo ainda é amplamente utilizado.</li>
                <li><strong>TLS (Transport Layer Security):</strong> Sucessor do SSL, oferece criptografia e autenticação mais robustas. TLS garante a segurança na comunicação, protegendo dados contra espionagem e ataques.</li>
            </ul>
            <p><strong>Métodos HTTP:</strong></p>
            <ul>
                <li><strong>GET:</strong> Solicita dados de um servidor. <br> Exemplo: Quando você visita <code>https://www.exemplo.com</code>, o navegador envia uma requisição GET para obter a página web.</li>
                <li><strong>POST:</strong> Envia dados ao servidor para criar ou atualizar um recurso. <br> Exemplo: Ao preencher um formulário de registro e enviá-lo, o navegador usa POST para enviar os dados e criar uma nova conta de usuário.</li>
                <li><strong>PUT:</strong> Substitui ou adiciona um recurso no servidor. Se o recurso não existir, é criado; se existir, é substituído. <br> Exemplo: Enviando uma requisição PUT para <code>https://api.exemplo.com/usuarios/123</code> com novos dados, o servidor atualiza ou cria o usuário com ID 123.</li>
                <li><strong>DELETE:</strong> Remove um recurso do servidor. <br> Exemplo: Enviando uma requisição DELETE para <code>https://api.exemplo.com/usuarios/123</code>, o servidor remove o usuário com ID 123.</li>
                <li><strong>PATCH:</strong> Faz alterações parciais em um recurso existente. <br> Exemplo: Enviando uma requisição PATCH para <code>https://api.exemplo.com/usuarios/123</code> para atualizar apenas o endereço de e-mail do usuário.</li>
            </ul>
            <p><strong>Códigos de Status HTTP:</strong></p>
            <ul>
                <li><strong>200 OK:</strong> Solicitação bem-sucedida.</li>
                <li><strong>404 Not Found:</strong> Recurso não encontrado.</li>
                <li><strong>500 Internal Server Error:</strong> Erro no servidor.</li>
            </ul>
        </section>

        <section>
            <h2>3. Domínio</h2>
            <p><strong>Definição:</strong> Nome que identifica um site na web, facilitando a navegação. <br> Exemplo: <code>www.exemplo.com</code> é um nome de domínio que leva a um site específico.</p>
        </section>

        <section>
            <h2>4. IP (Endereço IP)</h2>
            <p><strong>Definição:</strong> Identificador numérico único para cada dispositivo na rede. <br> Exemplo: Um endereço IP pode ser <code>192.168.1.1</code>, identificando um dispositivo específico.</p>
        </section>

        <section>
            <h2>5. Host</h2>
            <p><strong>Definição:</strong> Computador ou servidor que armazena e fornece acesso a sites e serviços. <br> Exemplo: Um servidor web que hospeda um site é um host.</p>
        </section>

        <section>
            <h2>6. DNS (Sistema de Nomes de Domínio)</h2>
            <p><strong>Definição:</strong> Sistema que traduz nomes de domínio em endereços IP. <br> Exemplo: O DNS converte <code>www.exemplo.com</code> em um endereço IP como <code>93.184.216.34</code> para que os navegadores possam encontrar o site.</p>
        </section>

        <section>
            <h2>7. Cliente-Servidor</h2>
            <p><strong>Modelo Cliente-Servidor:</strong> Estrutura onde clientes solicitam serviços e servidores fornecem respostas.</p>
            <p><strong>Exemplos:</strong></p>
            <ul>
                <li><strong>Navegação na Web:</strong> Navegador (cliente) solicita páginas web; servidor envia as páginas.</li>
                <li><strong>E-mail:</strong> Cliente de e-mail envia mensagens para um servidor de e-mail que entrega as mensagens.</li>
            </ul>
        </section>

        <section>
            <h2>8. Redes e Topologias</h2>
            <p><strong>Redes:</strong></p>
            <ul>
                <li><strong>LAN (Rede Local):</strong> Conecta dispositivos em uma área limitada.</li>
                <li><strong>WAN (Rede de Longa Distância):</strong> Conecta redes em locais distantes.</li>
            </ul>
            <p><strong>Topologias:</strong></p>
            <ul>
                <li><strong>Topologia em Estrela:</strong> Dispositivos conectados a um ponto central.</li>
                <li><strong>Topologia em Malha:</strong> Dispositivos interconectados, oferecendo múltiplos caminhos.</li>
            </ul>
        </section>

        <section>
            <h2>9. Navegadores e Servidores Web</h2>
            <p><strong>Navegadores:</strong> Softwares que interpretam e exibem páginas web (Chrome, Firefox, etc.).</p>
            <p><strong>Servidores Web:</strong> Programas que armazenam e fornecem páginas web para navegadores.</p>
        </section>

        <section>
            <h2>10. Segurança na Internet</h2>
            <p><strong>Criptografia:</strong> Métodos de proteger dados através de codificação para segurança durante a transmissão.</p>
            <p><strong>Proteção Contra Ataques:</strong></p>
            <ul>
                <li><strong>Phishing:</strong> Engana usuários para obter informações pessoais.</li>
                <li><strong>Malware:</strong> Software malicioso para causar danos ou roubar informações.</li>
            </ul>
        </section>
    </div>
</body>
</html>
