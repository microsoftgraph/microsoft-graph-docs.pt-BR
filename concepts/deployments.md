# <a name="sovereign-cloud-deployments"></a>Implantações de nuvem soberana


Este artigo fornece informações sobre as diferentes instâncias da nuvem soberana do Microsoft Graph e os recursos que estão disponíveis para os desenvolvedores. 


## <a name="microsoft-graph-operated-by-21vianet-in-china"></a>Microsoft Graph operado pela 21Vianet na China

Esta seção fornece informações sobre o Microsoft Graph operado pela 21Vianet e os recursos que estão disponíveis para os desenvolvedores. 

### <a name="microsoft-graph-service-root-endpoints"></a>Pontos de extremidade de raiz do serviço do Microsoft Graph
| Microsoft Graph operado pela 21Vianet | Microsoft Graph|
|---------------------------|----------------|
| https://microsoftgraph.chinacloudapi.cn | https://graph.microsoft.com|

### <a name="microsoft-graph-explorer"></a>Microsoft Graph Explorer
| Microsoft Graph Explorer na China | Microsoft Graph Explorer|
|---------------------------|----------------|
|https://graph.microsoft.io/zh-cn/graph-explorer| https://graph.microsoft.io/en-us/graph-explorer|

### <a name="azure-openid-connect-and-oauth20"></a>OpenID Connect e OAuth2.0 do Azure
Os pontos de extremidade usados para adquirir tokens para entrar ou para chamar o Microsoft Graph operado pelo 21Vianet são diferentes de outras ofertas. 

| Microsoft Graph operado pela 21Vianet | Microsoft Graph|
|---------------------------|----------------|
| https://login.chinacloudapi.cn | https://login.microsoftonline.com|
 
Use https://login.chinacloudapi.cn/common/oauth2/authorize para autenticar o usuário e https://login.chinacloudapi.cn/common/oauth2/token para adquirir um token para seu aplicativo para chamar o Microsoft Graph operado pela 21Vianet.

> **Observação:** os últimos [pontos de extremidade de token e autorização do v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview/) NÃO estão disponíveis para o uso com o Microsoft Graph operado pela 21Vianet. 

>Os aplicativos só podem acessar dados organizacionais e não os dados de clientes por meio do ponto de extremidade **https://microsoftgraph.chinacloudapi.cn**. Os aplicativos devem usar o ponto de extremidade **https://graph.microsoft.com** para acessar dados de clientes.

### <a name="service-capabilities-offered-by-microsoft-graph-operated-by-21vianet"></a>Recursos de serviço oferecidos pelo Microsoft Graph operado pela 21Vianet
Os seguintes recursos do Microsoft Graph estão disponíveis de maneira geral (no ponto de extremidade do `/v1.0`):

* Usuários
* Grupos
* Arquivos
* Email
* Calendário
* Contatos pessoais 
* CRUD (criar, ler, atualizar e excluir) operações
* Suporte a CORS (compartilhamento de recursos entre origens).

Os seguintes recursos do Microsoft Graph também estão disponíveis no modo de visualização (no ponto de extremidade do `/beta`):

* Contatos organizacionais
* Aplicativos
* Entidades de serviço
* Extensões de esquema de diretório
* Webhooks
