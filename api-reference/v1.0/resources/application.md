---
title: tipo de recurso do aplicativo
description: Representa um aplicativo.
ms.localizationpriority: high
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 8b7864114f357ea031fbaae72c8ee20ad6c477c3
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461188"
---
# <a name="application-resource-type"></a>tipo de recurso do aplicativo

Namespace: microsoft.graph

Representa um aplicativo. Qualquer aplicativo que terceirize a autenticação no Azure Active Directory (Azure AD) deve estar registrado em um diretório. O registro do aplicativo envolve informar o Azure AD sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, o URI para identificar seu aplicativo e muito mais. Para saber mais, confira [Noções básicas de como registrar um aplicativo no Azure AD](/azure/active-directory/develop/authentication-vs-authorization#basics-of-registering-an-application-in-azure-ad). Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/application-delta.md). Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar aplicativos](../api/application-list.md) | Coleção [application](application.md) | Recuperar a lista de aplicativos na organização. |
|[Criar aplicativo](../api/application-post-applications.md) | [application](application.md) | Cria (registra) um novo aplicativo.|
|[Obter aplicativo](../api/application-get.md) | [application](application.md) |Ler as propriedades e as relações de um objeto de aplicativo.|
|[Atualizar aplicativo](../api/application-update.md) | Nenhum |Atualize o objeto application. |
|[Excluir aplicativo](../api/application-delete.md) | Nenhum |Exclua o objeto application. |
|[Obter delta](../api/application-delta.md)|[aplicativo](application.md)|Obtenha os aplicativos recentemente criados, atualizados ou excluídos sem ter que executar uma leitura completa de toda a coleção de recursos.|
|[Listar aplicativos excluídos](../api/directory-deleteditems-list.md) | Conjunto [directoryObject](directoryobject.md) | Recuperar uma lista de aplicativos excluídos recentemente. |
| [Lista de aplicativos excluídos pertencentes a usuários](../api/directory-deleteditems-user-owned.md) | Coleção [directoryObject](directoryobject.md) | Recupere os aplicativos excluídos no locatário nos últimos 30 dias e que pertencem a um usuário. |
|[Obter o aplicativo excluído](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Recuperar as propriedades de um aplicativo excluído recentemente. |
|[Excluir aplicativo permanentemente](../api/directory-deleteditems-delete.md) | Nenhum | Excluir permanentemente um aplicativo. |
|[Restaurar aplicativo excluído](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | Restaurar um aplicativo excluído recentemente. |
|**Certificados e segredos**| | |
|[Adicionar senha](../api/application-addpassword.md)|[passwordCredential](passwordcredential.md)|Adicionar uma senha forte a um aplicativo.|
|[Remover senha](../api/application-removepassword.md)|[passwordCredential](passwordcredential.md)|Remover uma senha de um aplicativo.|
|[Adicionar chave](../api/application-addkey.md)|[keyCredential](keycredential.md)|Adicione uma credencial de chave a um aplicativo.|
|[Remover chave](../api/application-removekey.md)|Nenhum(a)|Remova uma credencial de chave de um aplicativo.|
|**Extensões**| | |
| [Listar extensionProperties](../api/application-list-extensionproperty.md) | Coleção [extensionProperty](extensionProperty.md) | Listar propriedades de extensão em um objeto de aplicativo. |
| [Criar extensionProperties](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Criar uma propriedade de extensão em um objeto de aplicativo. |
| [Obter extensionProperty](../api/extensionproperty-delete.md) | Nenhum | Obter uma propriedade de extensão de um objeto de aplicativo. |
| [Excluir extensionProperty](../api/extensionproperty-delete.md) | Nenhum | Excluir uma propriedade de extensão de um objeto de aplicativo. |
|[Obtenha as propriedades de extensão disponíveis](../api/directoryobject-getavailableextensionproperties.md)|Coleção [extensionProperty](../resources/extensionproperty.md)|Obtenha todas as listas ou uma lista filtrada das propriedades de extensão do diretório que foram registradas em um diretório.|
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

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#application-properties).

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| addIns | Coleção [addIn](addin.md)| Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](/onedrive/developer/file-handlers) para a funcionalidade "FileHandler". Isso permitirá que serviços como o Office 365 chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando. |
| api | [apiApplication](apiapplication.md) | Especifica configurações para um aplicativo que implementa uma API Web. |
| appId | Cadeia de caracteres | O identificador exclusivo para o aplicativo que está atribuído a um aplicativo pelo Microsoft Azure Active Directory. Não anulável. Somente leitura. |
| applicationTemplateId | String | Identificador exclusivo do applicationTemplate. Apoia `$filter` (`eq`, `not`, `ne`).|
| appRoles | Coleção [appRole](approle.md) | O conjunto de funções atribuídas ao aplicativo. Com as [atribuições de funções do aplicativo](approleassignment.md), essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos. Não anulável. |
| createdDateTime | DateTimeOffset | A data e a hora em que o aplicativo foi registrado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. <br><br> Dá suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`e `eq` em `null` valores ) e `$orderBy`. |
| deletedDateTime | DateTimeOffset | A data e a hora em que o aplicativo foi excluído. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
| description | Cadeia de caracteres | Campo de texto livre para fornecer uma descrição do objeto de aplicativo aos usuários finais. O tamanho máximo permitido é de 1.024 caracteres. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`) e `$search`. |
| disabledByMicrosoftStatus | Cadeia de caracteres | Especifica se a Microsoft desabilitou o aplicativo registrado. Os valores possíveis são: `null`(valor padrão), `NotDisabled` e (os motivos podem incluir atividades suspeitas, abusivas ou mal-intencionadas ou uma violação do `DisabledDueToViolationOfServicesAgreement` Contrato de Serviços Microsoft). <br><br> Suporta `$filter` (`eq`, `ne`, `not`). |
| displayName | String | O nome de exibição do aplicativo. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$search`, e `$orderBy`. |
| groupMembershipClaims | Cadeia de caracteres | Configura a declaração `groups` emitida em um usuário ou token de acesso OAuth 2.0 que o aplicativo espera. Para definir esse atributo, use um dos seguintes valores da cadeia de caracteres válidos: `None`, `SecurityGroup` (para grupos de segurança e funções do Azure Active Directory), `All` (obtém todos os grupos de segurança, grupos de distribuição e diretório do Azure Active Directory funções das quais o usuário conectado é membro). |
| id | String | O identificador exclusivo do aplicativo. Herdado [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. Dá suporte `$filter`(`eq`, `ne`, `not`, `in`).|
| identifierUris | Coleção de cadeias de caracteres | Também conhecido como URI de ID do aplicativo, esse valor é definido quando um aplicativo é usado como um aplicativo de recurso. O identifierUris age como o prefixo para os escopos que você referencia no código da API e deve ser globalmente exclusivo. Você pode usar o valor padrão fornecido, que está no formato `api://<application-client-id>`, ou especificar um URI mais acessível como `https://contoso.com/api` . Para obter mais informações sobre padrões e práticas recomendadas de identificadorUris válidos, consulte [Práticas recomendadas de segurança de registro de aplicativos do Azure AD](/azure/active-directory/develop/security-best-practices-for-app-registration#appid-uri-configuration). Não anulável. <br><br>Suporta `$filter` (`eq`, `ne`, `ge`, `le`, `startsWith`).|
| informações  | [informationalUrl](informationalurl.md) | Informações básicas de perfil do aplicativo, como marketing, suporte, termos de serviço e URLs de política de privacidade do aplicativo. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, confira [Como adicionar termos de serviço e política de privacidade a aplicativos do Azure AD registrados](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). <br><br>Dá suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`e `eq` em `null` valores). |
| isDeviceOnlyAuthSupported | Booliano | Especifica se este aplicativo dá suporte à autenticação de dispositivo sem um usuário. O padrão é `false`.  |
| isFallbackPublicClient | Booliano | Especifica o tipo de aplicativo de fallback como cliente público; por exemplo, um aplicativo instalado em um dispositivo móvel. O valor padrão é `false`, o que significa que o tipo de aplicativo de fallback é cliente confidencial, como um aplicativo web. No entanto, há situações em que o Azure AD não consegue determinar o tipo de aplicativo cliente. Por exemplo, o fluxo [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) onde o aplicativo está configurado sem especificar um URI de redirecionamento. Nesses casos, o Azure AD interpretará o tipo de aplicativo com base no valor dessa propriedade.|
| keyCredentials | [keyCredential](keycredential.md) collection | A coleção de credenciais de chave associadas ao aplicativo. Não anulável. Dá suporte `$filter`(`eq`, `not`, `ge`, `le`). |
| logo | Stream | O logotipo principal do aplicativo. Não anulável. |
| notes | String | Anotações relevantes para o gerenciamento do aplicativo. |
| oauth2RequiredPostResponse | Boolean | Especifica se, como parte das solicitações de token OAuth 2.0, o Azure AD permite solicitações POST, em vez de solicitações GET. O padrão é `false`, que especifica que somente as solicitações GET são permitidas. |
| optionalClaims | [optionalClaims](optionalclaims.md) | Os desenvolvedores de aplicativos podem configurar declarações opcionais em seus aplicativos do Azure AD para especificar as declarações enviadas ao aplicativo pelo serviço de token de segurança da Microsoft. Para obter mais informações, consulte [Como fornecer declarações opcionais ao seu aplicativo](/azure/active-directory/develop/active-directory-optional-claims).|
| parentalControlSettings | [parentalControlSettings](parentalcontrolsettings.md) |Especifica as configurações de controle parental de um aplicativo. |
| passwordCredentials | [passwordCredential](passwordcredential.md) collection|A coleção de credenciais de senha associadas ao aplicativo Não anulável.|
| publicClient | [publicClientApplication](publicclientapplication.md) | Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho. |
| publisherDomain | String | O domínio do publicador verificado para o aplicativo. Somente leitura. Para obter mais informações, consulte [Como: configurar o domínio do publisher de um aplicativo](/azure/active-directory/develop/howto-configure-publisher-domain). Suporta `$filter` (`eq`, `ne`, `ge`, `le`, `startsWith`).|
| requiredResourceAccess |[requiredResourceAccess](requiredresourceaccess.md) collection| Especifique os recursos que o aplicativo precisa acessar. Essa propriedade também especifica o conjunto de permissões delegadas e funções de aplicativo necessárias para cada um desses recursos. Essa configuração de acesso aos recursos necessários impulsiona a experiência de consentimento. Não é possível configurar mais de 50 APIs (serviços de recursos). A partir de meados de outubro de 2021, o número total de permissões necessárias não deve exceder 400. Não anulável. <br><br>Suporta `$filter` (`eq`, `not`, `ge`, `le`).|
| referênciaDeGerenciamentoDeServiços | Cadeia de caracteres | Faz referências de aplicativo ou informações de contato de serviço de um banco de dados de Gerenciamento de Serviços ou Ativos. Anulável. |
| signInAudience | Cadeia de caracteres | Especifique quais contas Microsoft têm suporte para o aplicativo atual. Os valores possíveis são: `AzureADMyOrg`, `AzureADMultipleOrgs`, `AzureADandPersonalMicrosoftAccount` (padrão) e `PersonalMicrosoftAccount`. Confira mais na [tabela abaixo](#signinaudience-values). <br><br>Suporta `$filter` (`eq`, `ne`, `not`).|
| spa                     | [spaApplication](../resources/spaapplication.md)                            | Especifica as configurações de um aplicativo de página simples, incluindo URLs de saída e de redirecionamento de URIs para os códigos de autorização e tokens de acesso. |
| categorias |Coleção String| Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulada.<br><br>Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
| tokenEncryptionKeyId |Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD criptografa todos os tokens emitidos usando a chave para a qual essa propriedade aponta. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | Especifica o editor verificado do aplicativo. Para obter mais informações sobre como a verificação do editor ajuda a dar suporte à segurança, confiabilidade e conformidade do aplicativo, consulte [Verificação do fornecedor](/azure/active-directory/develop/publisher-verification-overview).|
| web |[webApplication](webapplication.md)| Especifica configurações para um aplicativo Web. |

### <a name="signinaudience-values"></a>signInAudience values

| Valor | Descrição |
|:---------------|:--------|
|AzureADMyOrg|Usuários com uma conta de corporativa ou estudante da Microsoft no locatário do Azure Active Directory da minha organização (locatário único).|
|AzureADMultipleOrgs|Usuários com uma conta de trabalho ou escola da Microsoft em qualquer locatário do Azure Active Directory (multilocatário) da organização.|
|AzureADandPersonalMicrosoftAccount|: Usuários com uma conta Microsoft pessoal, corporativa ou de estudante no locatário do Azure Active Directory de qualquer organização. Para autenticar usuários com fluxos de usuário do Active Directory B2C, use o `AzureADandPersonalMicrosoftAccount`. Este valor permite o mais amplo conjunto de identidades de usuário, incluindo contas locais e identidades de usuário da Microsoft, Facebook, Google, Twitter ou qualquer provedor de conexão OpenID. Este é o valor padrão para a propriedade **signInAudience**. |
|PersonalMicrosoftAccount|Usuários com uma conta Microsoft pessoal apenas.|

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Somente leitura.|
|extensionProperties|Coleção [extensionProperty](extensionproperty.md)| Somente leitura. Anulável. Dá suporte a `$expand` e `$filter` (`eq` ao contar as coleções vazias).|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários do aplicativo. Somente leitura. Nullable. Dá `$expand`.|

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
  "applicationTemplateId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "disabledByMicrosoftStatus": "String",
  "displayName": "String",
  "groupMembershipClaims": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isDeviceOnlyAuthSupported": false,
  "isFallbackPublicClient": false,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "notes": "String",
  "oauth2RequiredPostResponse": false,
  "optionalClaims": {"@odata.type": "microsoft.graph.optionalClaims"},
  "parentalControlSettings": {"@odata.type": "microsoft.graph.parentalControlSettings"},
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "serviceManagementReference": "String",
  "signInAudience": "String",
  "spa": {"@odata.type": "microsoft.graph.spaApplication"},
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
