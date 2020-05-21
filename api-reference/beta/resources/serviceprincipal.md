---
title: Tipo de recurso servicePrincipal
description: Representa uma instância de um aplicativo em um diretório. Herda do directoryObject.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: fc46c88d2ec676ac313602c279683da2c483deba
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336717"
---
# <a name="serviceprincipal-resource-type"></a>Tipo de recurso servicePrincipal

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma instância de um aplicativo em um diretório. Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/serviceprincipal-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[List servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) collection | Recupere uma lista de objetos servicePrincipal. |
|[Criar o servicePrincipalName](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | Cria um novo objeto servicePrincipalName. |
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Leia as propriedades e as relações do objeto servicePrincipal.|
|[Atualizar o servicePrincipalName](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Atualize o objeto servicePrincipal. |
|[Excluir o servicePrincipalName](../api/serviceprincipal-delete.md) | Nenhum |Exclua o objeto servicePrincipal.|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto createdObject.|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto ownedObject.|
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal collection| Obtenha alterações incrementais para entidades de serviço. |
|**Atribuições de função de aplicativo**| | |
|[List appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) collection| Obtenha as funções de aplicativo que esta entidade de serviço recebeu.|
|[Adicionar appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Atribua uma função de aplicativo a essa entidade de serviço.|
|[Remover appRoleAssignment](../api/serviceprincipal-delete-approleassignments.md) | Nenhum | Remova uma atribuição de função de aplicativo desta entidade de serviço.|
|[Listar appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md) |[appRoleAssignment](approleassignment.md) collection| Obtenha as funções de aplicativo atribuídas aos usuários, grupos e entidades de serviço para esta entidade de serviço.|
|[Adicionar appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| Atribua uma função de aplicativo para esta entidade de serviço a um usuário, grupo ou entidade de serviço.|
|[Remover appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md) | Nenhum | Remova uma atribuição de função de aplicativo para esta entidade de serviço de um usuário, grupo ou entidade de serviço.|
|**Certificados e segredos**| | |
|[Adicionar senha](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|Adicione uma senha forte a um servicePrincipalName.|
|[Remover senha](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|Remover uma senha de um servicePrincipalName.|
|[Tecla Adicionar](../api/serviceprincipal-addkey.md)|[keycredential](keycredential.md)|Adicione uma credencial de chave a um servicePrincipalName.|
|[Remover chave](../api/serviceprincipal-removekey.md)|Nenhum|Remover uma credencial de chave de um servicePrincipalName.|
|**Subsídios de permissão delegada**| | |
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) collection| Obtenha a permissão delegada que concede a autorização dessa entidade de serviço para acessar uma API em nome de um usuário conectado.|
|**Associação**| | |
|[Listar memberOf](../api/serviceprincipal-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Obtenha grupos dos quais essa entidade de serviço é membro direto da propriedade de navegação memberOf.|
|[List transitive memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) collection| Liste os grupos dos quais essa entidade de serviço é membro. Essa operação é transitiva e inclui os grupos dos quais essa entidade de serviço é um membro aninhado. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Conjunto de cadeias de caracteres|Verifique se há associação em uma lista de grupos específica.|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|Coleção de cadeias de caracteres|Verifique se há associação em uma lista de grupo específica, função de diretório ou objetos de unidade administrativa.|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String collection|Obtenha a lista de grupos dos quais essa entidade de serviço é membro.|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String collection|Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.|
|**Owners**| | |
|[Listar proprietários](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto owner.|
|[Adicionar proprietário](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Crie um novo proprietário postando na coleção owners.|
|[Remover proprietário](../api/serviceprincipal-delete-owners.md) |Nenhum| Remover um proprietário de um servicePrincipalName.|
|**Políticas**| | |
|[List assigned policies](../api/policy-list-assigned.md)| Coleção [policy](policy.md)| Obtenha todas as políticas atribuídas a esse objeto.|
|[Atribuir claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md)| Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)| Atribua um claimsMappingPolicy a este objeto.|
|[Listar claimsMappingPolicies](../api/serviceprincipal-list-claimsmappingpolicies.md)| Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)| Obter todos os claimsMappingPolicies atribuídos a este objeto.|
|[Remover claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md)| Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)| Remover um tokenLifetimePolicy deste objeto.|
|[Atribuir homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)| Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Atribuir um homeRealmDiscoveryPolicy a este objeto.|
|[Listar homeRealmDiscoveryPolicies](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)| Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Obter todos os homeRealmDiscoveryPolicies atribuídos a este objeto.|
|[Remover homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md)| Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Remover um homeRealmDiscoveryPolicy deste objeto.|
|[Atribiur tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md)| Atribuir um tokenLifetimePolicy a este objeto.|
|[Listar tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)| Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md)| Obter todos os tokenLifetimePolicies atribuídos a este objeto.|
|[Remover tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md)| Remover um tokenLifetimePolicy deste objeto.|
|**Logon único**| | |
|[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Crie uma credencial definida para o usuário ou grupo especificado no corpo.|
|[getPasswordSingleSignOnCredentials](../api/serviceprincipal-getpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Obtenha um conjunto de credenciais para o usuário ou grupo especificado no corpo.|
|[updatePasswordSingleSignOnCredentials](../api/serviceprincipal-updatepasswordsinglesignoncredentials.md)|Nenhum|Atualize um conjunto de credenciais para o usuário ou grupo especificado no corpo.|
|[deletePasswordSingleSignOnCredentials](../api/serviceprincipal-deletepasswordsinglesignoncredentials.md)|Nenhum|Exclua uma credencial definida para o usuário ou grupo especificado no corpo.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| **True** se a entidade de serviço estiver habilitada; caso contrário, **false**.|
| addIns | coleção [AddIn](addin.md) | Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler". Isso permitirá que serviços como o Office 365 chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando.|
|alternativos|Conjunto de cadeias de caracteres| Usado para recuperar entidades de serviço por assinatura, identificar grupo de recursos e IDs de recursos completos para [identidades gerenciadas](https://aka.ms/azuremanagedidentity).|
|appDisplayName|Cadeia de caracteres|O nome de exibição exposto pelo aplicativo associado.|
|appId|String|O identificador exclusivo do aplicativo associado (sua propriedade **appId**).|
|applicationTemplateId|String|Identificador exclusivo do applicationtemplate a partir do qual o servicePrincipalName foi criado. Somente leitura.|
|appOwnerOrganizationId|String|Contém a ID do locatário onde o aplicativo está registrado. Isso é aplicável somente a entidades de serviço apoiadas por aplicativos.|
|appRoleAssignmentRequired|Boolean|Especifica se os usuários ou outras entidades de serviço precisam receber uma atribuição de função de aplicativo para esta entidade de serviço para que os usuários possam entrar ou os aplicativos possam obter tokens. O valor padrão é **false**. Não anulável. |
|appRoles|Coleção [appRole](approle.md)|As funções expostas pelo aplicativo que esta entidade de serviço representa. Para obter mais informações, confira definição da propriedade **appRoles** na entidade [aplicativo](application.md). Não anulável. |
| deletedDateTime | DateTimeOffset | A data e a hora em que a entidade de serviço foi excluída. Somente leitura. |
|displayName|Cadeia de caracteres|O nome de exibição da entidade de serviço.|
|errorUrl|String|Obsoleto. Não use.|
|homepage|String|Página inicial ou página de aterrissagem do aplicativo.|
| id | String | O identificador exclusivo da entidade de serviço. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
| informações  | [informationalUrl](informationalurl.md) | Informações básicas de perfil do aplicativo adquirido, como marketing do aplicativo, suporte, termos de serviço e URLs da declaração de privacidade. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, confira [Como adicionar termos de serviço e política de privacidade a aplicativos do Azure AD registrados](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
|keyCredentials|[keyCredential](keycredential.md) collection|A coleção de credenciais principais associada à entidade de serviço. Não anulável.            |
|loginUrl|String|Especifica a URL na qual o provedor de serviços redireciona o usuário para o Azure AD autenticar. O Azure AD usa a URL para iniciar o aplicativo do Office 365 ou do Azure AD meus aplicativos. Quando estiver em branco, o Azure AD executará o logon iniciado pelo IdP para aplicativos configurados com o [logon único baseado em SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). O usuário inicia o aplicativo do Office 365, do Azure AD meus aplicativos ou da URL de SSO do Azure AD.|
|logoutUrl|String| Especifica a URL que será usada pelo serviço de autorização da Microsoft para efetuar logoff de um usuário usando os protocolos OpenId Connect [front-Channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-](https://openid.net/specs/openid-connect-backchannel-1_0.html) Channel ou logout SAML.|
|notificationEmailAddresses|Conjunto de cadeias de caracteres|Especifica a lista de endereços de email onde o Azure AD envia uma notificação quando o certificado ativo está próximo da data de vencimento. Isso se aplica apenas aos certificados usados para assinar o token SAML emitido para aplicativos da galeria do Azure AD.|
|passwordCredentials|[passwordCredential](passwordcredential.md) collection|A coleção de credenciais de senha associada à entidade de serviço. Não anulável. |
|preferredSingleSignOnMode|string|Especifica o modo de logon único configurado para este aplicativo. O Azure AD usa o modo de logon único preferencial para iniciar o aplicativo do Office 365 ou do Azure AD meus aplicativos. Os valores com suporte são password, SAML, external e oidc.|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|Especifica a data de expiração da keycredential usada para assinatura de token, marcada por **preferredTokenSigningKeyThumbprint**.|
|preferredTokenSigningKeyThumbprint|String|Reservado apenas para uso interno. Não escreva ou dependa de alguma forma dessa propriedade. Pode ser removida em versões futuras. |
|publishedPermissionScopes|coleção [permissionScope](permissionscope.md)|As permissões delegadas expostas pelo aplicativo. Para obter mais informações, consulte a propriedade **oauth2PermissionScopes** na propriedade **API** da entidade de [aplicativo](application.md) . Não anulável.|
|replyUrls|String collection|As URLs às quais os tokens de usuário são enviados para entrar com aplicativo associado ou os URIs de redirecionamento aos quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado. Não anulável. |
|samlMetadataUrl|String|A URL onde o serviço expõe metadados SAML para Federação.|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](samlsinglesignonsettings.md)|A coleção para configurações relacionadas ao logon único do SAML.|
|servicePrincipalNames|String collection|Contém a lista de **identifiersUris**, copiadas do [aplicativo](application.md)associado. Valores adicionais podem ser adicionados aos aplicativos híbridos. Esses valores podem ser usados para identificar as permissões expostas por este aplicativo no Azure AD. Por exemplo,<ul><li>Os aplicativos cliente podem especificar um URI de recurso que se baseia nos valores dessa propriedade para adquirir um token de acesso, que é o URI retornado na declaração "AUD".</li></ul><br>O operador any é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável.|
|servicePrincipalName|String|Identifica se a entidade de serviço representa um aplicativo ou uma identidade gerenciada. Isso é definido pelo Azure AD internamente. Para uma entidade de serviço que representa um [aplicativo](./application.md) , isso é definido como __aplicativo__. Para uma entidade de serviço que representa uma [identidade gerenciada](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview) , isso é definido como __ManagedIdentity__.|
|signInAudience|String| Especifica quais contas da Microsoft são compatíveis com o aplicativo associado. Somente leitura.|
|tags|Coleção String| Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar a entidade de serviço. Não anulável. |
|tokenEncryptionKeyId|Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD emite tokens para esse aplicativo criptografado usando a chave especificada por essa propriedade. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|

## <a name="relationships"></a>Relacionamento

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Entidades (usuários, grupos e entidades de serviço) que são atribuídas a essa entidade de serviço. Somente leitura.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Aplicativos aos quais esta entidade de serviço é atribuída. Somente leitura. Anulável.|
|createdObjects|[directoryObject](directoryobject.md) collection|Objetos de diretório criados pela entidade de serviço. Somente leitura. Anulável.|
|pontos de extremidade|conjunto [ponto de extremidade](endpoint.md) |Pontos de extremidade disponíveis para descoberta. Os serviços como o SharePoint esenchem essa propriedade com um locatário específico do SharePoint pontos de extremidade que outros aplicativos podem descobrir e usar em suas experiências.|
|memberOf|[directoryObject](directoryobject.md) collection|Funções das quais essa entidade de serviço é membro. Métodos HTTP: GET somente leitura. Anulável.|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) collection|Permissão delegada concede a autorização dessa entidade de serviço para acessar uma API em nome de um usuário conectado. Somente leitura. Anulável.|
|ownedObjects|[directoryObject](directoryobject.md) collection|Objetos de diretório que pertencem a essa entidade de serviço. Somente leitura. Anulável.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários desse servicePrincipalName. Os proprietários são um conjunto de usuários não administradores ou de servicePrincipalName que têm permissão para modificar esse objeto. Somente leitura. Anulável.|
|política|[policy](policy.md) collection|As políticas atribuídas a essa entidade de serviço.|
|claimsMappingPolicies|Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)|O claimsMappingPolicies atribuído a essa entidade de serviço.|
|homeRealmDiscoveryPolicies|Conjunto [homeRealmDiscoveryPolicy](homeRealmDiscoveryPolicy.md)|O homeRealmDiscoveryPolicies atribuído a essa entidade de serviço.|
|tokenLifetimePolicies|Conjunto [tokenLifetimePolicy](tokenLifetimePolicy.md)|O tokenLifetimePolicies atribuído a essa entidade de serviço.|

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "endpoints",
    "memberOf",
    "oauth2PermissionGrants",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipal"
}-->

```json
{
  "accountEnabled": true,
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "alternativeNames": "string",
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "applicationTemplateId": "string",
  "appRoleAssignmentRequired": true,
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "loginUrl": "string",
  "logoutUrl": "string",
  "notificationEmailAddresses": ["string"],
  "publishedPermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preferredSingleSignOnMode": "string",
  "preferredTokenSigningKeyEndDateTime": "DateTime",
  "preferredTokenSigningKeyThumbprint": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "samlSingleSignOnSettings": "microsoft.DirectoryServices.SamlSingleSignOnSettings",
  "servicePrincipalNames": ["string"],
  "servicePrincipalType": "string",
  "signInAudience": "String",
  "tags": ["string"],
  "tokenEncryptionKeyId": "String",
  "useCustomTokenSigningKey": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
