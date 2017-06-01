# <a name="get-access-tokens-to-call-microsoft-graph"></a>Obter tokens de acesso para chamar o Microsoft Graph

Para chamar o Microsoft Graph, seu aplicativo deve adquirir um token de acesso do Azure Active Directory (Azure AD), o serviço de identidade em nuvem da Microsoft. O token de acesso contém informações (ou declarações) sobre seu aplicativo e as permissões que ele possui para os recursos e APIs disponíveis no Microsoft Graph. Para obter um token de acesso, o aplicativo deve ser capaz de se autenticar com o Azure AD e ter a autorização de um usuário ou administrador para acessar os recursos necessários do Microsoft Graph. 

Este tópico fornece uma visão geral dos tokens de acesso, do Azure AD e de como seu aplicativo pode obter tokens de acesso. Se você já estiver familiarizado com a integração de um aplicativo com o Azure AD para obter tokens, avance para as [Próximas Etapas](#next-steps) para obter informações e exemplos específicos do Microsoft Graph. 

## <a name="what-is-an-access-token-and-how-do-i-use-it"></a>O que é um token de acesso e como usá-lo?

Os tokens de acesso emitidos pelo Azure AD são JWT (Token Web JSON) codificado em base 64. Eles contêm informações (declarações) que as APIs da Web protegidas pelo Azure AD, como o Microsoft Graph, usam para validar o chamador e para garantir que o chamador tenha as permissões adequadas para executar a operação solicitada. Ao chamar o Microsoft Graph, você pode tratar os tokens de acesso como opacos. Você deve sempre transmitir tokens de acesso em canais seguros, como protocolo TLS (HTTPS).

Veja um exemplo de um token de acesso do Azure AD:

`EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/oeJX6U8nnL9nJ5pHLVuPWD0aNnTPTJD8Y4oQTp5zLhDIIfaJCaGcQperULVF7K6yX8MhHxIBwek418rKIp11om0SWBXOYSGOM0rNNN59qNiKwLNK+MPUf7ObcRBN5I5vg8jB7IMoz66jrNmT2uiWCyI8MmYDZgAACPoaZ9REyqke+AE1/x1ZX0w7OamUexKF8YGZiw+cDpT/BP1GsONnwI4a8M7HsBtDgZPRd6/Hfqlq3HE2xLuhYX8bAc1MUr0gP9KuH6HDQNlIV4KaRZWxyRo1wmKHOF5G5wTHrtxg8tnXylMc1PKOtaXIU4JJZ1l4x/7FwhPmg9M86PBPWr5zwUj2CVXC7wWlL/6M89Mlh8yXESMO3AIuAmEMKjqauPrgi9hAdI2oqnLZWCRL9gcHBida1y0DTXQhcwMv1ORrk65VFHtVgYAegrxu3NDoJiDyVaPZxDwTYRGjPII3va8GALAMVy5xou2ikzRvJjW7Gm3XoaqJCTCExN4m5i/Dqc81Gr4uT7OaeypYTUjnwCh7aMhsOTDJehefzjXhlkn//2eik+NivKx/BTJBEdT6MR97Wh/ns/VcK7QTmbjwbU2cwLngT7Ylq+uzhx54R9JMaSLhnw+/nIrcVkG77Hi3neShKeZmnl5DC9PuwIbtNvVge3Q+V0ws2zsL3z7ndz4tTMYFdvR/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==`

Para chamar o Microsoft Graph, anexe o token de acesso como um token de portador ao cabeçalho de autorização em uma solicitação HTML. Por exemplo, veja uma chamada que retorna as informações de perfil do usuário conectado (o token de acesso foi truncado para facilitar a leitura):

```
HTTP/1.1
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
Host: graph.microsoft.com`
GET https://graph.microsoft.com/v1.0/me/
```

## <a name="what-are-microsoft-graph-permissions"></a>O que são as permissões do Microsoft Graph?
O Microsoft Graph expõe um conjunto valioso de permissões granulares sobre os recursos que ele controla. Essas permissões são expressadas como cadeias de caracteres e concedem aplicativos de acesso a recursos do Microsoft Graph, como usuários, grupos, email de usuário, etc. Por exemplo:

- _User.Read_ permite que um aplicativo leia o perfil do usuário conectado.
- _Mail.Send_ permite que um aplicativo envie emails em nome do usuário conectado.

Há dois tipos de permissões:

- As Permissões delegadas são usadas pelos aplicativos que são executados com um usuário presente. Os privilégios de usuário são delegados ao aplicativo que faz chamadas para o Microsoft Graph em nome do usuário. Muitas dessas permissões podem ser consentidas por um usuário, mas outras exigem consentimento do administrador.  
- As Permissões de aplicativo são usadas pelos aplicativos que são executados sem um usuário. Elas geralmente concedem amplos privilégios a um aplicativo dentro de uma organização e exigem sempre o consentimento de um administrador.

Para obter uma lista completa das permissões do Microsoft Graph, além das diferenças entre as Permissões delegadas e Permissões de aplicativo, confira a [Referência de permissões](permissions_reference.md).

## <a name="where-does-my-app-get-an-access-token"></a>Onde meu aplicativo pode obter um token de acesso?
Seu aplicativo adquire tokens de acesso do Azure Active Directory (Azure AD), o serviço de identidade em nuvem da Microsoft. Para obter um token de acesso, o aplicativo troca respostas e solicitações HTTP com o Azure AD usando protocolos padrão da indústria definidos nas especificações do OAuth 2.0 e do OpenID Connect 1.0. Esses protocolos descrevem os pontos de extremidade do Azure AD e as trocas com eles, ou fluxos de autenticação, que seu aplicativo usa para se autenticar de forma segura com o Azure AD e obter tokens de acesso.  

Em um nível muito simples, para obter um token de acesso, seu aplicativo troca solicitações HTTP com os seguintes pontos de extremidade:

- O ponto de extremidade `/authorize` no qual seu aplicativo pode enviar um usuário para autenticar-se com o Azure AD e concordar com as permissões de seu aplicativo.
- O ponto de extremidade `/token` no qual seu aplicativo pode obter um token de acesso depois que o consentimento do usuário for concedido.

(Observação: Essas definições não são rígidas. Dependendo do protocolo usado pelo aplicativo, ele pode obter tokens de acesso diretamente do ponto de extremidade `/authorize` ou ele pode se autenticar diretamente no ponto de extremidade `/token`.) 

Veja um exemplo de um conjunto de pontos de extremidade `/authorize` e `/token` expostos pelo Azure AD v2.0:

```
https://login.microsoftonline.com/common/oauth2/v2.0/authorize
https://login.microsoftonline.com/common/oauth2/v2.0/token

```
O Azure AD expõe dois conjuntos de pontos de extremidade, o Azure AD e o Azure AD v2.0. A principal diferença entre eles é que o ponto de extremidade do Azure AD só dá suporte a contas corporativas e de estudante (ou seja, contas associadas a um locatário do Azure AD), enquanto que o Azure AD v2.0 também dá suporte a contas da Microsoft como _Live.com_ ou _outlook.com_. Isso significa que, se você usar o ponto de extremidade do Azure AD, seu aplicativo só poderá segmentar organizações, mas com o Azure AD v2.0, poderá segmentar clientes e organizações. 

Os tokens do ponto de extremidade do AD do Azure não são intercambiáveis com os do ponto de extremidade do Azure AD v2.0, portanto, antes de começar a trabalhar em um aplicativo para produção, você deve escolher entre os pontos de extremidade. Como o ponto de extremidade do Azure AD v2.0 é mais recente e os recursos ainda estão sendo adicionados, existem algumas limitações importantes que você precisa considerar na decisão sobre qual ponto de extremidade deve ser usado no aplicativo na produção. Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Azure AD e do Azure AD v2.0](#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

## <a name="whats-the-difference-between-oauth-20-and-openid-connect"></a>Qual é a diferença entre o OAuth 2.0 e o OpenID Connect?

O OAuth 2.0 é um protocolo de autorização. Ele define como seu aplicativo pode obter tokens de acesso, autenticando-se diretamente no Azure AD ou redirecionando um usuário para autenticar-se no Azure AD e concordar com as permissões solicitadas pelo aplicativo. No primeiro caso, seu aplicativo obtém um token de acesso que ele pode usar para chamar o Microsoft Graph como ele próprio. No segundo caso, seu aplicativo obtém um token de acesso que ele pode usar para chamar o Microsoft Graph em nome de um usuário. No entanto, com o OAuth 2.0, seu aplicativo não recebe informações sobre o usuário ou como ele foi autenticado pelo Azure AD. Os fluxos do OAuth 2.0 geralmente são mais usados por aplicativos móveis ou nativos que já conhecem a identidade do usuário, ou por aplicativos, como serviços em segundo plano ou daemons, que chamam o Microsoft Graph com sua própria identidade e não em nome de um usuário.

O OpenID Connect estende o OAuth 2.0 para fornecer uma camada de identidade. Com o OpenID Connect, além de um token de acesso, seu aplicativo também pode obter um token de identificação do Azure AD. Os tokens de identificação do OpenID Connect contêm declarações sobre a identidade do usuário e detalhes sobre como e onde eles foram autenticados. Os fluxos do OpenID Connect são normalmente usados por aplicativos Web, incluindo aplicativos de uma única página (SPAs). Esses aplicativos podem usar o token de identificação para personalizar seu comportamento para o usuário para o qual eles solicitaram um token de acesso e, em muitos casos, terceirizar o logon de seus usuários para o Azure AD e permitir experiências como o logon único (SSO).

## <a name="what-kind-of-apps-can-i-call-microsoft-graph-from"></a>De que tipos de aplicativos posso chamar o Microsoft Graph?
Você pode chamar o Microsoft Graph a partir dos seguintes tipos de aplicativos: 

- **Aplicativos nativos**: Aplicativos que são executados em um dispositivo como uma área de trabalho, tablet ou celular. Esses aplicativos usam o sistema operacional (SO) nativo do dispositivo como o iOS, o Android ou o Windows na apresentação do usuário e fazer chamadas para o Microsoft Graph em nome de um usuário.
- **Aplicativos Web**: Aplicativos que são executados em um servidor e interagem com o usuário conectado por meio de um usuário-agente, geralmente um navegador da Web. A maior parte da camada de apresentação é tratada no servidor e as chamadas para o Microsoft Graph são feitas do lado do servidor em nome de um usuário.
- **Aplicativos de Página Única (SPA)**: Aplicativos Web com experiências de usuário valiosas que lidam com grande parte da camada de apresentação através de scripts do lado do cliente no navegador. As chamadas para o Microsoft Graph são feitas a partir do script do cliente usando tecnologias como AJAX e estruturas como o Angular.js. As chamadas são feitas em nome de um usuário.
- **Daemons/Serviços em segundo plano**: Serviços em segundo plano e daemons que são executados em um servidor sem a presença de um usuário e fazer chamadas para o Microsoft Graph com sua própria identidade.
- **APIs da Web**: Um aplicativo de cliente chama uma API da Web (protegida pelo Azure AD) que, em seguida, chama o Microsoft Graph, tudo em nome de um usuário. Compatível com o ponto de extremidade do Azure AD. No caso do ponto de extremidade do Azure AD v2.0, só terá suporte se o cliente e a API da Web tiverem a mesmo Id de Aplicativo. Por exemplo, um aplicativo nativo que chama um back-end da API da Web. 

## <a name="how-do-i-get-my-app-talking-to-azure-ad-and-microsoft-graph"></a>Como fazer com que meu aplicativo se comunique com o Azure AD e o Microsoft Graph?
Seu aplicativo deve estar registrado antes de poder obter um token do Azure AD. Para o ponto de extremidade do Azure AD v2.0, use o [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) para registrar seu aplicativo. No caso do ponto de extremidade do Azure AD, use o [Portal do Azure](https://azure.portal.com/). O registro integra seu aplicativo com o Azure AD e estabelece as coordenadas e identificadores usados para obter tokens. Eles são:

- **Id do aplicativo**: Um identificador exclusivo atribuído pelo Azure AD. 
- **URI/URL de redirecionamento**: Um ou mais pontos de extremidade no qual seu aplicativo receberá respostas do Azure AD. (Para aplicativos móveis e nativos, será um URI atribuído pelo Azure AD.)
- **Segredo do Aplicativo**: Uma senha ou um par de chaves públicas/particulares que seu aplicativo usa para se autenticar no Azure AD. (Não é necessário para aplicativos nativos ou móveis.)

Para aplicativos que usam o ponto de extremidade do Azure AD, você também pré-configurará as permissões do Microsoft Graph que seu aplicativo usará durante o registro. Para aplicativos que usam o ponto de extremidade do Azure AD v2.0, pode ou não ser necessário pré-configurar permissões. 

As propriedades definidas durante o registro são usadas na conexão. Por exemplo, na solicitação de token a seguir: *client_id* é o *Id do aplicativo*, *redirect_uri* é um de seus *URIs de redirecionamento* e *client_secret* é o *Segredo do Aplicativo*. 

```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

## <a name="are-there-authentication-libraries-available"></a>Há bibliotecas de autenticação disponíveis?
Como a maioria dos desenvolvedores, você provavelmente usará bibliotecas de autenticação para gerenciar suas interações com o Azure AD. As bibliotecas de autenticação abstraem muitos detalhes do protocolo, como validação, manipulação de cookies, armazenamento de token em cache e manutenção de conexões seguras, fora do desenvolvedor e isso permite que você focalize seu desenvolvimento no aplicativo. A Microsoft publica bibliotecas de cliente de código-fonte aberto e middleware de servidor para os pontos de extremidade do Azure AD e do Azure AD v2.0. 

Para o ponto de extremidade do Azure AD v2.0: 

- As bibliotecas de cliente da Biblioteca de Autenticação da Microsoft (MSAL) estão disponíveis para .NET, JavaScript, Android e Objective-c. Todas as plataformas estão em pré-visualização com suporte à produção e, no caso de alterações serem introduzidas, a Microsoft garante um caminho para a atualização.
- O middleware de servidor da Microsoft está disponível para .NET core e ASP.NET (OWIN OpenID Connect e OAuth) e para Node.js (Microsoft Azure AD Passport.js). 
- O ponto de extremidade v2.0 é compatível com várias bibliotecas de autenticação de terceiros.

Para obter uma lista completa de bibliotecas de cliente da Microsoft, middleware de servidor da Microsoft e bibliotecas de terceiros compatíveis, confira [Bibliotecas de autenticação do Azure Active Directory v2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).

Para o ponto de extremidade do Azure AD:

- As bibliotecas de cliente da ADAL (Active Directory Authentication Library) estão disponíveis em um número um pouco maior de plataformas. 
- O middleware de servidor da Microsoft está disponível para .NET core e ASP.NET, além de Node.js. 

Para obter uma lista completa de bibliotecas de cliente da Microsoft e middleware de servidor, confira [Bibliotecas de Autenticação do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).

## <a name="deciding-between-the-azure-ad-and-azure-ad-v20-endpoints"></a>Decidindo entre os pontos de extremidade do Azure AD e do Azure AD v2.0

O Azure AD expõe dois conjuntos de pontos de extremidade, o Azure AD e o Azure AD v2.0, onde você pode obter tokens de acesso para usar ao chamar o Microsoft Graph. Os tokens recebidos de cada ponto de extremidade não são intercambiáveis. Para executar exemplos ou explorar a funcionalidade do Microsoft Graph, a escolha dos pontos de extremidade do Azure AD não é essencial. No entanto, antes de iniciar o desenvolvimento em um aplicativo de produção, você precisa decidir qual ponto de extremidade fará mais sentido para seu cenário. A discussão a seguir fornece algumas diretrizes gerais que podem ser usadas para ajudar na tomada de decisão, mas, para informações mais atuais e abrangentes, você deve consultar [Devo usar o ponto de extremidade do v2.0?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations) na documentação do Azure Active Directory. 

A principal diferença entre o Azure AD e o Azure AD v2.0 é que:

* O Azure AD só é compatível com contas corporativa ou de estudante, ou seja, contas associadas a um locatário do Azure AD. Isso significa que seu aplicativo pode direcionar somente para organizações.
* O Azure AD v2.0 é compatível com contas corporativas e de estudante e contas da Microsoft como contas _live.com_ ou _outlook.com_. Isso significa que seu aplicativo pode direcionar para clientes e organizações que usam o ponto de extremidade do v2.0. 

O Azure AD v2.0 oferece mais algumas vantagens. Por exemplo:

* O aplicativo pode usar uma única Id de Aplicativo para várias plataformas. Isso simplifica o gerenciamento do aplicativo para desenvolvedores e administradores.
* [Suporte para consentimento dinâmico e incremental](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare#incremental-and-dynamic-consent). Com esse recurso, seu aplicativo pode solicitar permissões adicionais durante o tempo de execução, emparelhando o pedido de consentimento do usuário com a funcionalidade que o requer. Isso proporciona uma experiência muito mais confortável para os usuários do que ter que consentir com uma longa lista de permissões quando eles fizerem o logon pela primeira vez.  

Como o Azure AD v2.0 é mais recente do que o Azure AD e os recursos ainda estão sendo adicionados, existem algumas limitações no ponto de extremidade do v2.0 que você precisa incluir em sua decisão. Por exemplo:

* Alguns recursos podem ainda não ser totalmente implementados na versão 2.0. Por exemplo, o aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como [acesso condicional ao dispositivo](https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies).
* Não é possível chamar o Microsoft Graph a partir de uma [API da Web autônoma](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#restrictions-on-app-types). 
* Não é possível chamar aplicativos do provedor de Soluções na Nuvem.
* A [autenticação integrada do Windows para locatários federados](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#restrictions-for-work-and-school-accounts) não tem suporte. Isso significa que os usuários de locatários federados do Azure AD não podem autenticar silenciosamente com sua instância local do Active Directory. Eles terão que digitar as credenciais novamente.

Para obter mais informações sobre as diferenças entre o ponto de extremidade do Azure AD v2.0 e o ponto de extremidade do Azure AD, confira [O que há de diferente no ponto de extremidade do v2.0?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare).

>**Importante**
>
>**Antes de tomar uma decisão sobre qual ponto de extremidade usar ao desenvolver um aplicativo para produção, confira [Devo usar o ponto de extremidade v2.0?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations).**

## <a name="next-steps"></a>Próximas etapas

Depois de registrar seu aplicativo, você estará pronto para começar!

- Para obter etapas rápidas para obter um token de acesso para aplicativos que chamam o Microsoft Graph em nome de um usuário, confira [Obter acesso em nome dos usuários](auth_v2_user.md).
- Para obter etapas rápidas para obter um token de acesso para aplicativos que chamam o Microsoft Graph sem um usuário, confira [Obter acesso sem um usuário](auth_v2_user.md).
- Para ver as permissões que você pode usar com o Microsoft Graph, confira [Permissões](permissions_reference.md).
- Se você é um provedor de Soluções na Nuvem da Microsoft interessado em acessar dados de clientes gerenciados por parceiros por meio do Microsoft Graph, confira [Gerenciar o acesso ao aplicativo (CSPs)](auth_cloudsolutionprovider.md).


Se já estiver pronto para entrar no código, você pode usar os seguintes recursos para ajudá-lo a implementar a autenticação e a autorização com o Azure AD em seu aplicativo.

### <a name="microsoft-graph-connect-samples"></a>Exemplos de Conexão usando o Microsoft Graph 

A Microsoft publica exemplos do Connect para o Microsoft Graph para uma ampla variedade de plataformas, incluindo: Android, Angular.JS, ASP.NET, iOS (Obj-C e Swift), Node.JS, PHP, Python, Ruby, UWP e Xamarin. Você pode usar esses exemplos para examinar o código que utiliza diversas bibliotecas de autenticação para obter tokens do Azure AD. Atualmente, a maioria dos exemplos usa bibliotecas de autenticação de terceiros. No entanto, os exemplos de ASP.NET e UWP usam bibliotecas da Microsoft.

- A seção [Crie seu primeiro aplicativo](get-started.md) contém artigos detalhados que mostram como criar aplicativos do Connect usando o ponto de extremidade do Azure AD v2.0 e aborda as bibliotecas de autenticação usadas em cada plataforma. Os exemplos disponíveis estão listados por plataformas e pontos de extremidade de autenticação.
- Para obter um exemplo executado em sua plataforma preferida, confira [Início Rápido do Microsoft Graph](https://developer.microsoft.com/graph/Quick-Start).
- Visite o [repositório do Microsoft Graph](https://github.com/microsoftgraph) no GitHub para ver todos os exemplos disponíveis do Microsoft Graph. 

### <a name="azure-active-directory-samples-and-documentation"></a>Documentação e exemplos do Azure Active Directory 
A documentação do Azure AD contém artigos e exemplos que se concentram especificamente na autenticação e autorização no Azure AD.

Para o ponto de extremidade do Azure AD v2.0: 

- A [documentação do ponto de extremidade do Azure AD v2.0 ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview) é o melhor local para começar. Este artigo contém links para visualizações, documentação de protocolos e artigos de introdução para plataformas diferentes, todos organizados pelo tipo de aplicativo que você está desenvolvendo. 
- Para ver exemplos listados pela biblioteca de autenticação de cliente ou servidor, confira [Bibliotecas de Autenticação do Azure Active Directory v2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries). 
- Ou você pode explorar exemplos do Azure AD por plataformas na [galeria de Código do Azure](https://azure.microsoft.com/resources/samples/?service=active-directory). Observação: você não pode qualificar sua pesquisa pela versão do ponto de extremidade. 

Para o ponto de extremidade do Azure AD: 

- A [visão geral do guia do Desenvolvedor do Azure AD](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide) é o melhor local para começar. Este artigo contém links para visualizações, documentação de protocolos e artigos de introdução para plataformas diferentes, organizados pelo tipo de aplicativo que você está desenvolvendo. 
- Para ver exemplos listados pela biblioteca de autenticação de cliente ou servidor, confira [Bibliotecas de Autenticação do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries). 
- Para ver exemplos listados pelo tipo de aplicativo e plataforma, confira [Exemplos de Códigos do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-code-samples).
- Ou você pode explorar exemplos do Azure AD por plataformas na [galeria de Código do Azure](https://azure.microsoft.com/resources/samples/?service=active-directory). Observação: você não pode qualificar sua pesquisa pela versão do ponto de extremidade. 


## <a name="see-also"></a>Veja também

- [Documentação do ponto de extremidade do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)
- [Documentação do ponto de extremidade do Azure Active Directory v2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)
