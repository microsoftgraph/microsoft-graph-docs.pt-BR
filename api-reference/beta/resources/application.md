---
title: tipo de recurso do aplicativo
description: Representa um aplicativo.
localization_priority: Priority
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 84cb01ae1aaa32552bdc6069670cc696e6813e55
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134761"
---
# <a name="application-resource-type"></a>tipo de recurso do aplicativo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo. Qualquer aplicativo que terceirize a autenticação no Azure Active Directory (Azure AD) deve estar registrado em um diretório. O registro do aplicativo envolve informar o Azure AD sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, o URI para identificar seu aplicativo e muito mais. Para saber mais, confira [Noções básicas de como registrar um aplicativo no Azure AD](/azure/active-directory/develop/authentication-vs-authorization#basics-of-registering-an-application-in-azure-ad). Herda de [directoryObject](directoryobject.md).

> [!Note]
> Atualmente, as alterações no tipo de recurso do aplicativo estão em desenvolvimento. Para saber mais, confira [Problemas conhecidos do Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/application-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar aplicativos](../api/application-list.md) | Coleção [application](application.md) | Recuperar a lista de aplicativos na organização. |
|[Criar aplicativo](../api/application-post-applications.md) | [application](application.md) | Cria (registra) um novo aplicativo.|
|[Obter aplicativo](../api/application-get.md) | [application](application.md) |Ler as propriedades e as relações de um objeto de aplicativo.|
|[Atualizar aplicativo](../api/application-update.md) | [application](application.md) |Atualize o objeto application. |
|[Excluir aplicativo](../api/application-delete.md) | Nenhum |Exclua o objeto application. |
|[Listar aplicativos excluídos](../api/directory-deleteditems-list.md) | Conjunto [directoryObject](directoryobject.md) | Recuperar uma lista de aplicativos excluídos recentemente. |
|[Obter o aplicativo excluído](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Recuperar as propriedades de um aplicativo excluído recentemente. |
|[Excluir aplicativo permanentemente](../api/directory-deleteditems-delete.md) | Nenhum | Excluir permanentemente um aplicativo. |
|[Restaurar aplicativo excluído](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | Restaurar um aplicativo excluído recentemente. |
|[delta](../api/application-delta.md)|Coleção [application](application.md)| Obtenha alterações incrementais para aplicativos. |
|[Criar chamada](../api/application-post-calls.md)|[call](call.md)|Crie uma nova chamada postando na coleção calls.|
|[Criar reunião online](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Crie uma nova reunião online postando na coleção onlineMeetings.|
|**Certificados e segredos**| | |
|[Adicionar senha](../api/application-addpassword.md)|[passwordCredential](passwordcredential.md)|Adicionar uma senha forte a um aplicativo.|
|[Remover senha](../api/application-removepassword.md)|[passwordCredential](passwordcredential.md)|Remover uma senha de um aplicativo.|
|[Adicionar chave](../api/application-addkey.md)|[keyCredential](keycredential.md)|Adicione uma credencial de chave a um aplicativo.|
|[Remover chave](../api/application-removekey.md)|Nenhum(a)|Remova uma credencial de chave de um aplicativo.|
|**Extensões**| | |
| [Listar extensões](../api/application-list-extensionproperty.md) | Coleção [extensionProperty](extensionProperty.md) | Listar propriedades de extensão em um objeto de aplicativo. |
| [Criar extensão](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Criar uma propriedade de extensão em um objeto de aplicativo. |
| [Excluir extensão](../api/application-delete-extensionproperty.md) | Nenhum | Excluir uma propriedade de extensão de um objeto de aplicativo. |
|**Owners**| | |
|[Listar proprietários](../api/application-list-owners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objetos owner.|
|[Adicionar proprietário](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Adicionar um proprietário postando na coleção de proprietários.|
|[Remover proprietário](../api/application-delete-owners.md) |Nenhum| Remover um proprietário de um aplicativo.|
|**Políticas**| | |
|[Atribuir tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Atribuir um tokenIssuancePolicy a este objeto.|
|[Listar TokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Obter todos os tokenIssuancePolicies atribuídos a este objeto.|
|[Remover tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Remover um tokenIssuancePolicy deste objeto.|
|[Atribiur tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)| Atribuir um tokenLifetimePolicy a este objeto.|
|[Listar tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)| Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)| Obter todos os tokenLifetimePolicies atribuídos a este objeto.|
|[Remover tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)| Remover um tokenLifetimePolicy deste objeto.|
|**Distribuidor verificado**| | |
|[Definir distribuidor verificado](../api/application-setverifiedpublisher.md)| Nenhum | Definir o distribuidor verificado de um aplicativo.|
|[Desmarcar distribuidor verificado](../api/application-unsetverifiedpublisher.md)| Nenhum | Desmarcar o distribuidor verificado de um aplicativo.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| addIns | Coleção [addIn](addin.md) | Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler". Isso permitirá que serviços como o Office 365 chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando. |
| api | [apiApplication](apiapplication.md) | Especifica configurações para um aplicativo que implementa uma API Web. |
| appId | Cadeia de caracteres | O identificador exclusivo para o aplicativo que está atribuído a um aplicativo pelo Azure AD. Não anulável. Somente leitura. |
| appRoles | Coleção [appRole](approle.md) | O conjunto de funções atribuídas ao aplicativo. Com as [atribuições de funções do aplicativo](approleassignment.md), essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos. Não anulável. |
| createdDateTime | DateTimeOffset | A data e a hora que o aplicativo foi registrado. Somente leitura. |
| deletedDateTime | DateTimeOffset | A data e a hora que o aplicativo foi excluído. Somente leitura. |
| displayName | String | O nome de exibição do aplicativo. |
| groupMembershipClaims | Cadeia de caracteres | Configura a declaração `groups` emitida em um usuário ou o token de acesso OAuth 2.0 que o aplicativo espera. Para definir esse atributo, use um dos seguintes valores válidos de cadeia de caracteres:<ul><li>`None`</li><li>`SecurityGroup`: para grupos de segurança e funções do Azure AD</li><li>`All`: Isso obterá todos os grupos de segurança, de distribuição e funções de diretório do Azure AD dos quais o usuário conectado é membro.</li></ul> |
| id | String | O identificador exclusivo do aplicativo. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
| identifierUris | Coleção de cadeias de caracteres | Os URIs que identificam o aplicativo em seu locatário do Azure AD ou em um domínio personalizado verificado, se o aplicativo é multilocatário. Para saber mais, confira [Objetos de aplicativo e Objetos de entidade de serviço](/azure/active-directory/develop/app-objects-and-service-principals). O operador `any` é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável. |
| informações  | [informationalUrl](informationalurl.md) | Informações básicas de perfil do aplicativo, como marketing, suporte, termos de serviço e URLs de política de privacidade do aplicativo. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, confira [Como: Adicionar termos de serviço e política de privacidade a aplicativos registrados do Azure AD](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
| isFallbackPublicClient | Booliano | Especifica o tipo de aplicativo de fallback como cliente público; por exemplo, um aplicativo instalado em um dispositivo móvel. O valor padrão é `false`, o que significa que o tipo de aplicativo de fallback é cliente confidencial, como um aplicativo web. No entanto, há situações em que o Azure AD não consegue determinar o tipo de aplicativo cliente. Por exemplo, o fluxo [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) onde o aplicativo está configurado sem especificar um URI de redirecionamento. Nesses casos, o Azure AD interpretará o tipo de aplicativo com base no valor dessa propriedade.|
| keyCredentials | [keyCredential](keycredential.md) collection | A coleção de credenciais chaves associada ao aplicativo. Não anulável. |
| logo | Stream | O principal logotipo do aplicativo. Não anulável. |
| oauth2RequiredPostResponse | Boolean | Especifica se, como parte das solicitações de token OAuth 2.0, o Azure AD permite solicitações POST, em vez de solicitações GET. O padrão é `false`, que especifica que somente as solicitações GET são permitidas. |
| onPremisesPublishing |[onPremisesPublishing](onpremisespublishing.md)| Representa o conjunto de propriedades necessário para [configurar o Proxy de Aplicativo](/graph/application-proxy-configure-api) para este aplicativo. Configurar essas propriedades permite que você publique seu aplicativo local para acesso remoto seguro. |
| optionalClaims | [optionalClaims](optionalclaims.md) | Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações serão enviadas ao aplicativo pelo serviço de token de segurança da Microsoft. Para saber mais, confira [Como: Fornecer declarações opcionais ao aplicativo](/azure/active-directory/develop/active-directory-optional-claims).|
| parentalControlSettings | [parentalControlSettings](parentalcontrolsettings.md) |Especifica as configurações de controle parental de um aplicativo. |
| passwordCredentials | Coleção [passwordCredential](passwordcredential.md)|A coleção de credenciais de senha associada ao aplicativo. Não anulável.|
| publicClient | [publicClientApplication](publicclientapplication.md) | Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho. |
| publisherDomain | String | O domínio do publicador verificado para o aplicativo. Somente leitura.|
| requiredResourceAccess |[requiredResourceAccess](requiredresourceaccess.md) collection| Especifique os recursos que o aplicativo precisa acessar. Essa propriedade também especifica o conjunto de escopos de permissão OAuth e as funções de aplicativo necessários para cada um desses recursos. Essa configuração de acesso aos recursos necessários impulsiona a experiência de consentimento. Não anulável.|
| signInAudience | Cadeia de caracteres | Especifique quais contas Microsoft têm suporte para o aplicativo atual. Os valores com suporte são:<ul><li>`AzureADMyOrg`: Usuários com uma conta Microsoft corporativa ou de estudante no locatário do Azure AD da minha organização (locatário único)</li><li>`AzureADMultipleOrgs`: Usuários com uma conta Microsoft corporativa ou de estudante em locatário Azure AD de qualquer organização (multi locatário)</li><li>`AzureADandPersonalMicrosoftAccount`: Usuários com uma conta Microsoft pessoal, corporativa ou de estudante no locatário do Azure AD de qualquer organização.</li><li>`PersonalMicrosoftAccount`: Somente os usuários com uma conta Microsoft pessoal.</li></ul> |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | Especifica as configurações de um aplicativo de página simples, incluindo URLs de saída e de redirecionamento de URIs para os códigos de autorização e tokens de acesso. |
| categorias |Coleção String| Sequências personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulável.|
| tokenEncryptionKeyId |Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD criptografa todos os tokens emitidos usando a chave para a qual essa propriedade aponta. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | Especifica o fornecedor verificado para o aplicativo.|
| web |[webApplication](webapplication.md)| Especifica configurações para um aplicativo Web. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|calls           |Coleção [call](call.md)                   |Somente leitura. Anulável.|
|connectorGroup|[connectorGroup](connectorgroup.md)| O connectorGroup que o aplicativo está usando com o Proxy de aplicativo do Azure AD. Anulável.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Somente leitura.|
|extensionProperties|Coleção [extensionProperty](extensionproperty.md)| Somente leitura. Anulável.|
|onlineMeetings  |Coleção [onlineMeeting](onlinemeeting.md)|Somente leitura. Anulável.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários do aplicativo. Somente leitura. Anulável.|
|tokenLifetimePolicies|Coleção [tokenLifetimePolicy](tokenLifetimePolicy.md)|O tokenLifetimePolicies atribuído a esse aplicativo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "groupMembershipClaims": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": false,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "oauth2RequiredPostResponse": false,
  "optionalClaims": {"@odata.type": "microsoft.graph.optionalClaims"},
  "parentalControlSettings": {"@odata.type": "microsoft.graph.parentalControlSettings"},
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "tokenEncryptionKeyId": "String",
  "verifiedPublisher": {"@odata.type": "microsoft.graph.verifiedPublisher"},
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

