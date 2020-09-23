---
title: tipo de recurso do aplicativo
description: Representa um aplicativo.
localization_priority: Priority
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2f24d607da62d83a847632f6e09585030a684d12
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193425"
---
# <a name="application-resource-type"></a>tipo de recurso do aplicativo

Namespace: microsoft.graph

Representa um aplicativo. Qualquer aplicativo que terceirize a autenticação no Azure Active Directory (Azure AD) deve estar registrado em um diretório. O registro do aplicativo envolve informar o Azure AD sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, o URI para identificar seu aplicativo e muito mais. Para saber mais, confira [Noções básicas de como registrar um aplicativo no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/application-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar aplicativos](../api/application-list.md) | Coleção [application](application.md) | Recuperar a lista de aplicativos na organização. |
|[Criar aplicativo](../api/application-post-applications.md) | [application](application.md) | Cria (registra) um novo aplicativo.|
|[Obter aplicativo](../api/application-get.md) | [application](application.md) |Ler as propriedades e as relações de um objeto de aplicativo.|
|[Atualizar aplicativo](../api/application-update.md) | [application](application.md) |Atualize o objeto application. |
|[Excluir aplicativo](../api/application-delete.md) | Nenhum |Exclua o objeto application. |
|[Obter delta](../api/application-delta.md)|[aplicativo](application.md)|Obtenha os aplicativos recentemente criados, atualizados ou excluídos sem ter que executar uma leitura completa de toda a coleção de recursos.|
|[Listar aplicativos excluídos](../api/directory-deleteditems-list.md) | Conjunto [directoryObject](directoryobject.md) | Recuperar uma lista de aplicativos excluídos recentemente. |
|[Obter o aplicativo excluído](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Recuperar as propriedades de um aplicativo excluído recentemente. |
|[Excluir aplicativo permanentemente](../api/directory-deleteditems-delete.md) | Nenhum | Excluir permanentemente um aplicativo. |
|[Restaurar aplicativo excluído](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | Restaurar um aplicativo excluído recentemente. |
|**Certificados e segredos**| | |
|[Adicionar senha](../api/application-addpassword.md)|[passwordCredential](passwordcredential.md)|Adicionar uma senha forte a um aplicativo.|
|[Remover senha](../api/application-removepassword.md)|[passwordCredential](passwordcredential.md)|Remover uma senha de um aplicativo.|
|[Adicionar chave](../api/application-addkey.md)|[keyCredential](keycredential.md)|Adicione uma credencial de chave a um aplicativo.|
|[Remover chave](../api/application-removekey.md)|Nenhum(a)|Remova uma credencial de chave de um aplicativo.|
|**Extensões**| | |
| [Listar extensões](../api/application-list-extensionproperty.md) | Coleção [extensionProperty](extensionProperty.md) | Listar propriedades de extensão em um objeto de aplicativo. |
| [Criar extensão](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Criar uma propriedade de extensão em um objeto de aplicativo. |
| [Excluir extensão](../api/application-delete-extensionproperty.md) | Nenhum | Excluir uma propriedade de extensão de um objeto de aplicativo. |
|[Obtenha as propriedades de extensão disponíveis](../api/directoryobject-getavailableextensionproperties.md)|Coleção [extensionProperty](../resources/extensionproperty.md)|Obtenha todas as listas ou uma lista filtrada das propriedades de extensão do diretório que foram registradas em um diretório.|
|**Owners**| | |
|[Listar proprietários](../api/application-list-owners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objetos owner.|
|[Adicionar proprietário](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Adicionar um proprietário postando na coleção de proprietários.|
|[Remover proprietário](../api/application-delete-owners.md) |Nenhum| Remover um proprietário de um aplicativo.|
|**Políticas**| | |
|[Atribuir tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Atribuir um tokenIssuancePolicy a este objeto.|
|[Listar TokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Obter todos os tokenIssuancePolicies atribuídos a este objeto.|
|[Remover tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Remover um tokenIssuancePolicy deste objeto.|
|[Atribiur tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md)| Atribuir um tokenLifetimePolicy a este objeto.|
|[Listar tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)| Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md)| Obter todos os tokenLifetimePolicies atribuídos a este objeto.|
|[Remover tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md)| Remover um tokenLifetimePolicy deste objeto.|


## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| addIns | Coleção [addIn](addin.md)| Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler". Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando. |
| api | [apiApplication](apiapplication.md) | Especifica configurações para um aplicativo que implementa uma API Web. |
| appId | String | O identificador exclusivo para o aplicativo que está atribuído a um aplicativo pelo Azure AD. Não anulável. Somente leitura. |
| appRoles | Coleção [appRole](approle.md) | A coleção de funções que o aplicativo declara. Com as [atribuições de funções do aplicativo](approleassignment.md), essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos. Não anulável. |
| createdDateTime | DateTimeOffset | A data e a hora que o aplicativo foi registrado. Somente leitura. |
| deletedDateTime | DateTimeOffset | A data e a hora que o aplicativo foi excluído. Somente leitura. |
| displayName | String | O nome de exibição do aplicativo. |
| groupMembershipClaims | Cadeia de caracteres | Configura a declaração `groups` emitida em um usuário ou o token de acesso OAuth 2.0 que o aplicativo espera. Para definir esse atributo, use um dos seguintes valores válidos de cadeia de caracteres:<ul><li>`None`</li><li>`SecurityGroup`: para grupos de segurança e funções do Azure AD</li><li>`All`: isso obterá todos os grupos de segurança e de distribuição e funções de diretório do Azure AD dos quais o usuário conectado é membro.</li></ul> |
| id | String | O identificador exclusivo do aplicativo. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
| identifierUris | Coleção de cadeias de caracteres | Os URIs que identificam o aplicativo em seu locatário do Azure AD ou em um domínio personalizado verificado, se o aplicativo é multilocatário. Para saber mais, confira [Objetos de aplicativo e objetos de entidade de serviço](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals). O operador *any* é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável. |
| informações  | [informationalUrl](informationalurl.md) | Informações básicas de perfil do aplicativo, como marketing, suporte, termos de serviço e URLs de política de privacidade do aplicativo. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, confira [Como adicionar termos de serviço e política de privacidade a aplicativos do Azure AD registrados](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
| isFallbackPublicClient | Booliano | Especifica o tipo de aplicativo de fallback como cliente público; por exemplo, um aplicativo instalado em um dispositivo móvel. O valor padrão é `false`, o que significa que o tipo de aplicativo de fallback é cliente confidencial, como um aplicativo Web. Há determinados cenários em que o Azure AD não pode determinar o tipo de aplicativo cliente (por exemplo, o fluxo [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3), no qual ele é configurado sem especificar um URI de redirecionamento). Nesses casos, o Azure AD interpretará o tipo de aplicativo com base no valor dessa propriedade.|
| keyCredentials | Coleção [keyCredential](keycredential.md) | A coleção de credenciais chaves associada ao aplicativo Não anulável. |
| logo | Stream | O principal logotipo do aplicativo. Não anulável. |
| optionalClaims | [optionalClaims](optionalclaims.md) | Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft. Confira [fornecer declarações opcionais ao aplicativo Azure AD](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.|
| parentalControlSettings | [parentalControlSettings](parentalcontrolsettings.md) |Especifica as configurações de controle parental de um aplicativo. |
| passwordCredentials | Coleção [passwordCredential](passwordcredential.md)|A coleção de credenciais de senha associada ao aplicativo. Não anulável.|
| publicClient | [publicClientApplication](publicclientapplication.md) | Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho. |
| publisherDomain | String | O domínio do publicador verificado para o aplicativo. Somente leitura.|
| requiredResourceAccess |[requiredResourceAccess](requiredresourceaccess.md) collection|Especifica os recursos para os quais esse aplicativo requer acesso e o conjunto de escopos de permissão e funções de aplicativo do OAuth necessários em cada um desses recursos. Essa pré-configuração de acesso necessário aos recursos impulsiona a experiência de consentimento. Não anulável.|
| signInAudience | Cadeia de caracteres | Especifica a quais contas Microsoft têm suporte para o aplicativo atual. Os valores com suporte são:<ul><li>`AzureADMyOrg`: Usuários com uma conta Microsoft corporativa ou de estudante no locatário do Azure AD da organização (ou seja, locatário único)</li><li>`AzureADMultipleOrgs`: Usuários com uma conta Microsoft corporativa ou de estudante no locatário do Azure AD da organização (ou seja, multilocatário)</li><li>`AzureADandPersonalMicrosoftAccount`: Usuários com uma conta Microsoft pessoal, corporativa ou de estudante no locatário do Azure AD de qualquer organização.</li></ul> |
| categorias |Coleção String| Sequências personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulável.|
| tokenEncryptionKeyId |Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD criptografa todos os tokens emitidos usando a chave para a qual essa propriedade aponta. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|
| web |[webApplication](webapplication.md)| Especifica configurações para um aplicativo Web. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Somente leitura.|
|extensionProperties|Coleção [extensionProperty](extensionproperty.md)| Somente leitura. Anulável.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários do aplicativo. Os proprietários são um conjunto de usuários não administradores e que têm permissão para modificar esse objeto. Requer a versão 2013-11-08 ou mais recente. Somente leitura. Anulável.|

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
  "optionalClaims": {"@odata.type": "microsoft.graph.optionalClaims"},
  "parentalControlSettings": {"@odata.type": "microsoft.graph.parentalControlSettings"},
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "tokenEncryptionKeyId": "String",
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

