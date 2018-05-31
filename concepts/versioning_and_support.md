# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Controle de versão, suporte e mudanças significativas de políticas para o Microsoft Graph 

Este artigo descreve o suporte e as alterações significativas de políticas do Microsoft Graph e as versões da API Microsoft Graph disponível no momento.

## <a name="support-policy-and-deprecation-information"></a>Informações de política e substituição de suporte

O Microsoft Graph segue a [Política de Ciclo de Vida da Microsoft](https://support.microsoft.com/en-us/lifecycle). 

Conforme novas versões das APIs REST Microsoft Graph e SDKs do Microsoft Graph são lançadas, as versões anteriores são desativadas. A Microsoft declarará uma versão como preterida pelo menos 24 meses antes de retirar uma API ou um SDK. 

Quando incrementamos a versão principal da API (por exemplo, da v1.0 para a v2.0), estamos anunciando que a versão atual (neste exemplo, v1.0) está obsoleta imediatamente e não ofereceremos mais suporte 24 meses após o anúncio. Podemos fazer exceções a essa política em questões de segurança de serviço ou confiabilidade de integridade.  

Quando uma API é marcada como preterida, é altamente recomendável que você migre para a versão mais recente assim que possível. Em alguns casos, anunciaremos que os novos aplicativos deverão começar a usar as novas APIs um pouco depois das APIs originais serem preteridas. Nesses casos, apenas os aplicativos ativos que usam atualmente as APIs preteridas podem continuar a usá-las.   

### <a name="api-contract-and-non-backward-compatible-changes"></a>Contrato de API e alterações sem compatibilidade com versões anteriores

O Microsoft Graph tem um log de alterações entre as versões. Essas alterações estão listadas no [Log de alterações do Microsoft Graph](changelog.md). Conforme nova funcionalidade e dados são adicionados ao Microsoft Graph, incrementaremos o número de versão da API para qualquer alteração à API não compatível com versões anteriores. 

A seguir há exemplos de alterações não compatíveis com versões anteriores:

 - Mudanças na URL ou solicitação/resposta fundamentais associadas ao recurso    
 - Remoção, renomear ou alterar o tipo de uma propriedade declarada
 - Remoção ou renomeação de APIs ou parâmetros de API
 - Adição de um cabeçalho de solicitação obrigatório

A seguir há exemplos de alterações compatíveis com versões anteriores:

 - Adição de propriedades que são anuláveis ou têm um valor padrão
 - Adição de um membro a uma enumeração
 - Remover, renomear ou alterar o tipo de uma extensão aberta
 - Remover, renomear ou alterar o tipo de uma anotação
 - Introdução de paginação a coleções existentes
 - Alterações de códigos de erro
 - Alterações à ordem das propriedades
 - Alterações ao formato ou ao comprimento de cadeias de caracteres opacas, como IDs de recurso

>**Nota:** ao longo do tempo, atualizaremos a lista de alterações compatíveis com versões anteriores. Se você gerar seus próprios proxies de cliente (como clientes WCF), nossa orientação é que os aplicativos cliente devem estar preparados para receber propriedades e tipos derivados definidos anteriormente pelo serviço da API do Microsoft Graph. A API do Microsoft Graph segue a orientação descrita na seção [Controle de Versão de Modelo](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) nas [diretrizes da API REST da Microsoft](https://github.com/microsoft/api-guidelines/). 

## <a name="versions"></a>Versões

As seguintes versões da API Microsoft Graph estão disponíveis atualmente.

### <a name="beta-version"></a>Versão beta
Exposto em `https://graph.microsoft.com/beta`, a versão beta da API Microsoft Graph contém recursos que estão atualmente _**na visualização**_. Para obter a documentação da API beta, veja [Referência de ponto de extremidade do Microsoft Graph beta](../api-reference/beta/beta-overview.md). Espere alterações significativas na versão beta regularmente. Não haverá uma dependência de produção em APIs /beta.

Não damos nenhuma garantia de que um recurso beta será promovido para a versão atual. Quando a equipe da API Microsoft Graph acredita que um recurso beta está pronto para disponibilidade geral (GA), adicionaremos esse recurso à versão atual mais recente. Se a promoção do recurso resultar em uma alteração significativa de uma versão atual, o número da versão será incrementado e a nova versão se tornará a versão atual.
Nossa comunidade do desenvolvedor pode postar solicitação de recursos no [UserVoice](https://officespdev.uservoice.com/), incluindo solicitações de novos recursos, bem como solicitações para promover APIs beta existentes para a versão atual. 

### <a name="current-version"></a>Versão atual

A versão atual do Microsoft Graph é a 1.0. Exposta em `https://graph.microsoft.com/v1.0`, a versão da API Microsoft Graph /v1.0 contém recursos que estão geralmente disponíveis e prontos para uso em produção. Você pode procurar a documentação das APIs 1.0 no sumário.

### <a name="deprecated-and-unsupported-versions"></a>Versões preteridas e sem suporte

Não há atualmente nenhuma versão preterida da Microsoft Graph.

## <a name="terms-of-use"></a>Termos de uso

Ao usar as APIs Microsoft Graph, você concorda com os [Termos de Uso](../misc/terms-of-use.md). 

Seus comentários são importantes para nós. Junte-se a nós na página [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Marque suas perguntas com {MicrosoftGraph}.
