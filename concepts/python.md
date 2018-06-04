# <a name="get-started-with-microsoft-graph-in-a-python-app"></a>Introdução ao Microsoft Graph em um aplicativo Python 

Este artigo descreve as tarefas obrigatórias para ter um token de acesso do Azure AD e chamar o Microsoft Graph. Ele mostra passo a passo como [Enviar um email pelo Microsoft Graph do Python](https://github.com/microsoftgraph/python-sample-send-mail) e explica os principais conceitos que você implementa para usar a API do Microsoft Graph. O artigo descreve como acessar o Microsoft Graph usando chamadas diretas REST.

![Enviar itens de formulário](https://raw.githubusercontent.com/microsoftgraph/python-sample-send-mail/master/static/images/sendmail.png)

## <a name="choosing-an-authentication-library"></a>Escolher uma biblioteca de autenticação

Para fazer chamadas para o Microsoft Graph, o aplicativo deve ter um token de acesso válido do Azure Active Directory (Azure AD), o serviço de identidade na nuvem da Microsoft, e o token deve ser transmitido em um cabeçalho HTTP com cada chamada para a API REST do Microsoft Graph. A abordagem do Graph para autenticação é baseada nos padrões OAuth 2.0 e Open ID Connect, portanto exitem várias [bibliotecas de autenticação](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/active-directory-v2-libraries) para você implementar a autenticação no seu aplicativo.

A amostra abordada abaixo usa a biblioteca [Flask-OAuthlib](https://flask-oauthlib.readthedocs.io/en/latest/) para implementar o fluxo de trabalho [Concessão do Código de Autorização](https://tools.ietf.org/html/rfc6749#section-4.1) do OAuth 2.0, que é o fluxo de trabalho recomendado para aplicativos Web criados no Python. Confira mais informações sobre outras opções de autenticação em [Amostras de autenticação do Python para o Microsoft Graph](https://github.com/microsoftgraph/python-sample-auth).

## <a name="installing-and-running-the-send-mail-sample"></a>Instalar e executar a amostra send-mail

Para instalar e configurar a amostra de aplicativo, siga as instruções em [Instalar as amostras de REST do Python](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md). Para a amostra send-mail abordada abaixo, use este comando para clonar o repositório:

```git clone https://github.com/microsoftgraph/python-sample-send-mail.git```

Ao registrar o aplicativo conforme abordado nas [instruções de instalação](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md), lembre-se de incluir as permissões **User.Read** e **Mail.Send**, que são necessárias para essa amostra.

Depois de concluir a instalação/configuração, execute a amostra de aplicativo seguindo as instruções para [executar a amostra](https://github.com/microsoftgraph/python-sample-send-mail#running-the-sample).

## <a name="code-walkthrough"></a>Passo a passo do código

A seguir está uma visão geral sobre o [código-fonte](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py) para a amostra de aplicativo.

As primeiras linhas de código são as [importações](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L4-L32) para os módulos e pacotes do Python usados na amostra:

* O módulo **base64** da biblioteca padrão é usado para codificar anexos de email.
* O módulo **mimetypes** é usado para determinar o tipo MIME para anexos de arquivos.
* O módulo **os** fornece funcionalidade comum do sistema de arquivos.
* O módulo **pprint** da biblioteca padrão é usado para fazer o pretty-print de qualquer mensagem de erro enviada pelo Graph. Por exemplo, se você tentar enviar para um endereço de email inválido.
* O módulo **uuid** da biblioteca padrão é usado para gerar uma cadeia aleatória de 36 caracteres para identificar de forma exclusiva cada solicitação do Graph. Isso pode ser útil para fins de depuração.
* O pacote **flask** é a estrutura da Web para a amostra.
* A classe **OAuth** de **flask_oauthlib.client** é um wrapper em torno do aplicativo Flask que implementa o fluxo de trabalho de autenticação do OAuth 2.0.
* O módulo **config** contém as configurações de registro do aplicativo, conforme configuradas no processo de instalação acima.

Em seguida, [criamos um aplicativo do Flask](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L15-L17) e o [objeto cliente do Graph](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L19-L28), chamado **MSGRAPH**.

Após essas etapas de configuração inicial vêm três funções de manipulador de roteamento do Flask que implementam o fluxo de trabalho de autenticação: [homepage()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L30-L33), [login()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L35-L39) e [authorized()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L41-L48). Saiba mais sobre o fluxo de trabalho de autenticação na seção [Amostra de arquitetura](https://github.com/microsoftgraph/python-sample-auth#sample-architecture) do repositório de amostras de autenticação do Python.

O próximo manipulador de roteamento, [mailform()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L50-L83), é o formulário onde você especifica os destinatários, o assunto e o corpo do email. Observe que esta função também inclui nossas primeiras chamadas para o Graph, incluindo a recuperação do perfil do usuário e da foto do perfil, o upload da foto para o OneDrive e a criação de um link de compartilhamento. Os dados são [passados para o modelo mailform.html](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L77-L83), em que o destinatário, o assunto e o corpo podem ser editados antes de enviar a mensagem. 

Em seguida, está a função [send_mail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L85-L107), que envia o email e exibe a resposta da API do Graph. Ela usa uma função auxiliar sendmail(), transmitindo os parâmetros da cadeia de caracteres de consulta que foram postados do formulário:

```python
response = sendmail(client=MSGRAPH,
                    subject=flask.request.args['subject'],
                    recipients=flask.request.args['email'].split(';'),
                    body=flask.request.args['body'],
                    attachments=[profile_pic])
```

A função [get_token()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L109-L123) é usada pela instância do cliente Flask-OAuthlib (```MSGRAPH```) para obter um token de acesso sempre que fazemos chamadas para o Graph. O token de acesso é transmitido em um cabeçalho HTTP chamado **Autorização**, mas não é preciso lidar com isso no seu código. Você pode simplesmente fazer chamadas para o Graph por meio dos métodos verbais HTTP do cliente (por exemplo, get() ou post()), e a instância do cliente saberá chamar ```get_token()``` para obter um token, porque a função é [decorada](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L109-L109) com ```tokengetter```.

O restante da amostra consiste em funções auxiliares que simplificam as atividades comuns do Graph:

* [request_headers()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L114-L123) retorna um dicionário de cabeçalhos HTTP que são enviados com cada chamada ao Graph.
* [profile_photo()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L125-L154) 
* [sendmail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L156-L202) envia uma mensagem usando o ponto de extremidade ```me/microsoft.graph.sendMail```.
* [sharing_link()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L204-L221) cria um link de compartilhamento para um item especificado no OneDrive.
* [upload_file()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L223-L255) carrega um arquivo no OneDrive.

Você pode achar essas funções auxiliares úteis em outras aplicações.

## <a name="other-python-rest-samples"></a>Outras amostras REST do Python

Aqui estão algumas outras amostras do Python que demonstram como trabalhar com vários aspectos do Microsoft Graph:

* [Amostras de autenticação do Python para Microsoft Graph](https://github.com/microsoftgraph/python-sample-auth)
* [Trabalhar com respostas paginadas do Microsoft Graph no Python](https://github.com/microsoftgraph/python-sample-pagination)
* [Trabalhar com extensões abertas do Graph no Python](https://github.com/microsoftgraph/python-sample-open-extensions)
* [Conecte um aplicativo Web Python à API de Segurança](https://github.com/microsoftgraph/python-security-rest-sample)

[Envie uma questão](https://github.com/microsoftgraph/python-sample-auth/issues) para nos informar sobre uma amostra específica que você queira ver. Gostaríamos de ouvir seus comentários sobre qualquer cenário do Microsoft Graph que você queira criar no Python!

A API do Microsoft Graph é uma API unificadora muito poderosa que pode ser usada para interagir com todos os tipos de dados da Microsoft. Confira a [documentação de desenvolvedor](https://developer.microsoft.com/pt-BR/graph/docs/concepts/overview) ou o [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer) para explorar o que mais você pode realizar com o Microsoft Graph.
