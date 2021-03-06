---
title: Tipo de recurso servicePrincipal
description: Representa uma instância de um aplicativo em um diretório. Herda do directoryObject.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 50c73d642536b890937fe55e7d0181a81d406e98
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576278"
---
# <a name="serviceprincipal-resource-type"></a>Tipo de recurso servicePrincipal

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma instância de um aplicativo em um diretório. Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/serviceprincipal-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) collection | Recupere uma lista de objetos servicePrincipal. |
|[Criar servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | Cria um novo objeto servicePrincipal. |
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Leia as propriedades e as relações do objeto servicePrincipal.|
|[Atualizar servicePrincipal](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Atualize o objeto servicePrincipal. |
|[Excluir servicePrincipal](../api/serviceprincipal-delete.md) | Nenhum(a) |Exclua o objeto servicePrincipal.|
|[Listar createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto createdObject.|
|[Listar ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto ownedObject.|
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal collection| Obtenha alterações incrementais para entidades de serviço. |
|**Atribuição de funções do aplicativo**| | |
|[List appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) collection| Obtenha as funções de aplicativo às quais esta entidade de serviço foi atribuída.|
|[Adicionar uma atribuição de função do aplicativo](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Atribuir uma função de aplicativo a essa entidade de serviço.|
|[Remover uma atribuição de função do aplicativo](../api/serviceprincipal-delete-approleassignments.md) | Nenhum(a) | Remover uma atribuição de função de aplicativo dessa entidade de serviço.|
|[Listar appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md) |coleção [appRoleAssignment](approleassignment.md)| Obtenha os usuários, grupos e funções de aplicativo atribuídos a essa entidade de serviço.|
|[Adicionar appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| Atribuir uma função de aplicativo dessa entidade de serviço a um usuário, grupo ou entidade de serviço.|
|[Remover appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md) | Nenhum(a) | Remova uma atribuição de função de aplicativo dessa entidade de serviço de um usuário, grupo ou entidade de serviço.|
|**Certificados e segredos**| | |
|[Adicionar senha](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|Adicione uma senha forte a uma servicePrincipal.|
|[Remover senha](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|Remova uma senha de uma servicePrincipal.|
|[Adicionar chave](../api/serviceprincipal-addkey.md)|[keyCredential](keycredential.md)|Adicione uma credencial de chave a uma servicePrincipal.|
|[Remover chave](../api/serviceprincipal-removekey.md)|Nenhum(a)|Remova uma credencial de chave de uma servicePrincipal.|
|**Classificações de permissão delegada**| | |
|[Lista de classificações de permissão delegada](../api/serviceprincipal-list-delegatedpermissionclassifications.md) |Coleção [delegatedPermissionClassification](delegatedpermissionclassification.md)| Obtenha as classificações de permissão para permissões delegadas expostas por essa entidade de serviço.|
|[Adicionar classificações de permissão delegada](../api/serviceprincipal-post-delegatedpermissionclassifications.md) |[delegatedPermissionClassification](delegatedpermissionclassification.md) | Adicione uma classificação de permissão para uma permissão delegada exposta por essa entidade de serviço. |
|[Remover classificação de permissão delegada](../api/serviceprincipal-delete-delegatedpermissionclassifications.md) | Nenhum | Remova uma classificação de permissão para uma permissão delegada exposta por essa entidade de serviço.|
|**Concessões de permissão delegadas**| | |
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) collection| Obtenha as concessões de permissão delegadas que autorizam essa entidade de serviço a acessar uma API em nome de um usuário conectado.|
|**Associação**| | |
|[Listar memberOf](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) collection| Obtenha grupos dos quais essa entidade de serviço é membro direto da propriedade de navegação memberOf.|
|[List transitive memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) collection| Liste os grupos dos quais essa entidade de serviço é membro. Essa operação é transitiva e inclui os grupos dos quais essa entidade de serviço é um membro aninhado. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há associação em uma lista de grupos específica.|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|Coleção de cadeias de caracteres|Verifique se há associação em uma lista de grupo específica, função de diretório ou objetos de unidade administrativa.|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Coleção de cadeias de caracteres|Obtenha a lista de grupos dos quais essa entidade de serviço é membro.|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Coleção de cadeias de caracteres|Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.|
|**Owners**| | |
|[Listar proprietários](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto owner.|
|[Adicionar proprietário](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Crie um novo proprietário postando na coleção owners.|
|[Remover proprietário](../api/serviceprincipal-delete-owners.md) |Nenhum(a)| Remova um proprietário de uma servicePrincipal.|
|**Políticas**| | |
|[Atribuir claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md)| Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)| Atribua um claimsMappingPolicy a este objeto.|
|[Listar claimsMappingPolicies](../api/serviceprincipal-list-claimsmappingpolicies.md)| Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)| Obter todos os claimsMappingPolicies atribuídos a este objeto.|
|[Remover claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md)| Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)| Remova uma claimsMappingPolicy deste objeto.|
|[Atribuir homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)| Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Atribuir um homeRealmDiscoveryPolicy a este objeto.|
|[Listar homeRealmDiscoveryPolicies](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)| Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Obter todos os homeRealmDiscoveryPolicies atribuídos a este objeto.|
|[Remover homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md)| Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)| Remover um homeRealmDiscoveryPolicy deste objeto.|
|[Atribuir tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Atribuir um tokenIssuancePolicy a este objeto.|
|[Listar TokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Obter todos os tokenIssuancePolicies atribuídos a este objeto.|
|[Remover tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| coleção [tokenIssuancePolicy](tokenissuancepolicy.md)| Remover um tokenIssuancePolicy deste objeto.|
|[Atribiur tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)| Atribuir um tokenLifetimePolicy a este objeto.|
|[Listar tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)| Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)| Obter todos os tokenLifetimePolicies atribuídos a este objeto.|
|[Remover tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)| Remover um tokenLifetimePolicy deste objeto.|
|**Acesso único**| | |
|[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Crie uma credencial definida para o usuário ou grupo especificado no corpo.|
|[getPasswordSingleSignOnCredentials](../api/serviceprincipal-getpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|Obtenha um conjunto de credenciais para o usuário ou grupo especificado no corpo.|
|[updatePasswordSingleSignOnCredentials](../api/serviceprincipal-updatepasswordsinglesignoncredentials.md)|Nenhum|Atualize um conjunto de credenciais para o usuário ou grupo especificado no corpo.|
|[deletePasswordSingleSignOnCredentials](../api/serviceprincipal-deletepasswordsinglesignoncredentials.md)|Nenhum|Exclua uma credencial definida para o usuário ou grupo especificado no corpo.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| **True** se a entidade de serviço estiver habilitada; caso contrário, **false**.|
| addIns | Coleção [addIn](addin.md) | Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler". Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando.|
|alternativeNames|Coleção de cadeias de caracteres| Usado para recuperar entidades de serviço por assinatura, identificar grupo de recursos e IDs de recursos completos de [identidades gerenciadas](https://aka.ms/azuremanagedidentity).|
|appDescription|String|A descrição exposta pelo aplicativo associado.|
|appDisplayName|String|O nome de exibição exposto pelo aplicativo associado.|
|appId|String|O identificador exclusivo do aplicativo associado (sua propriedade **appId**).|
|applicationTemplateId|String|Identificador exclusivo do applicationTemplate do qual a servicePrincipal foi criada. Somente leitura.|
|appOwnerOrganizationId|Cadeia de caracteres|Contém a ID de locatário onde o aplicativo está registrado. Isso é aplicável apenas a entidades de serviço respaldadas por aplicativos.|
|appRoleAssignmentRequired|Booliano|Especifica se os usuários ou outras entidade de serviço precisam receber uma atribuição de função de aplicativo para essa entidade de serviço antes que os usuários possam entrar ou os aplicativos possam obter tokens. O valor padrão é **falso**. Não anulável. |
|appRoles|Coleção [appRole](approle.md)|As funções expostas pelo aplicativo que essa entidade de serviço representa. Para obter mais informações, confira definição da propriedade **appRoles** na entidade [aplicativo](application.md). Não anulável. |
| deletedDateTime | DateTimeOffset | A data e a hora em que a entidade de serviço foi excluída. Somente leitura. |
|description| String | Campo de texto disponível para fornecer uma descrição voltada para o usuário final interno da entidade de serviço. Os portais do usuário final, como [MyApps](/azure/active-directory/user-help/my-apps-portal-end-user-access), exibirão a descrição do aplicativo neste campo. O tamanho máximo permitido é de 1.024 caracteres.|
|displayName|String|O nome de exibição da entidade de serviço.|
|errorUrl|Cadeia de caracteres|Depreciado. Não usar.|
|homepage|String|Página inicial ou página de aterrissagem do aplicativo.|
| id | String | O identificador exclusivo da entidade de serviço. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
| informações  | [informationalUrl](informationalurl.md) | Informações básicas de perfil do aplicativo adquirido, como marketing, suporte, termos de serviço e URLs de política de privacidade do aplicativo. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, confira [Como adicionar termos de serviço e política de privacidade a aplicativos do Azure AD registrados](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
|keyCredentials|[keyCredential](keycredential.md) collection|A coleção de credenciais principais associada à entidade de serviço. Não anulável.            |
|loginUrl|String|Especifica a URL na qual o provedor de serviços redireciona o usuário para a autenticação do Azure AD. O Azure AD usa a URL para iniciar o aplicativo do Microsoft 365 ou o Azure AD My Apps. Quando em branco, o Azure AD executa o logon iniciado pelo IdP de aplicativos configurados com o [logon único baseado em SAML](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). O usuário inicia o aplicativo do Microsoft 365, o Azure AD My Apps ou a URL de SSO do Azure AD.|
|logoutUrl|Cadeia de caracteres| Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff OpenId Connect [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.|
|notes|String|Campo de texto disponível para capturar informações sobre o principal do serviço, normalmente usado para fins operacionais. O tamanho máximo permitido é de 1.024 caracteres.|
|NotificationEmailAddresses|Coleção de cadeias de caracteres|Especifica a lista de endereços de email para os quais o Azure AD envia uma notificação quando o certificado ativo está próximo da data de validade. Isso é apenas para os certificados usados ​​para assinar o token SAML emitido para aplicativos da Galeria do Azure AD.|
|passwordCredentials|[passwordCredential](passwordcredential.md) collection|A coleção de credenciais de senha associada à entidade de serviço. Não anulável. |
|passwordSingleSignOnSettings|[passwordSingleSignOnSettings](passwordsinglesignonsettings.md)|A coleção para configurações relacionadas a senha de acesso único. Utilize `$select=passwordSingleSignOnSettings` para fazer a çeitura da propriedade.. Somente leitura para [applicationTemplates](applicationTemplate.md) com exceção para ApplicationTemplates personalizados. |
|preferredSingleSignOnMode|cadeia de caracteres|Especifica o modo de logon único configurado para este aplicativo. O Azure AD usa o modo de logon único preferido para iniciar o aplicativo do Microsoft 365 ou o Azure AD My Apps. Os valores com suporte são: `password`, `saml`, `notSupported`, e `oidc`.|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|Especifica a data da expiração do keyCredential usado para a assinatura do token, marcado por **preferredTokenSigningKeyThumbprint**.|
|preferredTokenSigningKeyThumbprint|String|Reservado apenas para uso interno. Não escreva ou dependa de alguma forma dessa propriedade. Pode ser removida em versões futuras. |
|publishedPermissionScopes|coleção [permissionScope](permissionscope.md)|As permissões delegadas expostas pelo aplicativo. Para obter mais informações, confira a propriedade **oauth2PermissionScopes** na propriedade [api](application.md) da entidade **aplicativo**. Não anulável.|
|replyUrls|String collection|As URLs às quais os tokens de usuário são enviados para entrar com aplicativo associado ou os URIs de redirecionamento aos quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado. Não anulável. |
|samlMetadataUrl|Cadeia de caracteres|O url em que o serviço expõe os metadados SAML para federação.|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](samlsinglesignonsettings.md)|A coleção das configurações relacionadas ao logon único do SAML.|
|servicePrincipalNames|Coleção de cadeias de caracteres|Contém a lista de **identificadoresUris**, copiados do [aplicativo](application.md) associado. É possível adicionar valores adicionais aos aplicativos híbridos. Esses valores podem ser usados ​​para identificar as permissões apresentadas por esse aplicativo no Azure AD. Por exemplo,<ul><li>Os aplicativos cliente podem especificar um URI de recurso com base nos valores dessa propriedade para adquirir um token de acesso, que é o URI retornado na declaração "aud".</li></ul><br>O operador any é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável.|
|servicePrincipalType|Cadeia de caracteres|Identifica se a entidade de serviço representa um aplicativo ou uma identidade gerenciada. Isso é definido pelo Azure AD internamente. Para uma entidade de serviço que representa um [aplicativo](./application.md), isso é definido como __Aplicativo__. Para obter uma entidade de serviço que represente uma [identidade gerenciada](/azure/active-directory/managed-identities-azure-resources/overview), essa configuração é definida como __ManagedIdentity__.|
|signInAudience|Cadeia de caracteres| Especifica quais são as contas da Microsoft compatíveis com o aplicativo associado. Apenas leitura.|
|tags|Coleção de cadeias de caracteres| Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar a entidade de serviço. Não anulável. |
|tokenEncryptionKeyId|Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD emite tokens para este aplicativo criptografado usando a chave especificada por essa propriedade. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | Especifica o distribuidor verificado do aplicativo que essa entidade de serviço representa.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Atribuições de função de aplicativo ou serviço, concedidas a usuários, grupos e outras entidades de serviços.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Atribuição de função de aplicativo para outro aplicativo ou serviço, concedida a essa entidade de serviço.|
|claimsMappingPolicies|Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)|O claimsMappingPolicies atribuído a essa entidade de serviço.|
|createdObjects|[directoryObject](directoryobject.md) collection|Objetos de diretório criados pela entidade de serviço. Somente leitura. Anulável.|
|delegatedPermissionClassifications|Conjunto de [delegatedPermissionClassification](delegatedpermissionclassification.md)|As classificações de permissão para permissões delegadas expostas pelo aplicativo que essa entidade de serviço representa.|
|pontos de extremidade|coleção [ponto de extremidade](endpoint.md) |Pontos de extremidade disponíveis para descoberta. Serviços como o Sharepoint preenchem essa propriedade com pontos de extremidade do SharePoint específicos de locatários que outros aplicativos podem descobrir e usar em suas experiências.|
|homeRealmDiscoveryPolicies|Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)|O homeRealmDiscoveryPolicies atribuído a essa entidade de serviço.|
|memberOf|[directoryObject](directoryobject.md) collection|Funções das quais essa entidade de serviço é membro. Métodos HTTP: GET somente leitura. Anulável.|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) collection|Concessões de permissão delegadas que autorizam essa entidade de serviço a acessar uma API em nome de um usuário conectado. Somente leitura. Anulável.|
|ownedObjects|[directoryObject](directoryobject.md) collection|Objetos de diretório que pertencem a essa entidade de serviço. Somente leitura. Anulável.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários dessa servicePrincipal. Os proprietários são um conjunto de usuários não administradores ou servicePrincipal que têm permissão para modificar esse objeto. Somente leitura. Anulável.|
|tokenIssuancePolicies|coleção [tokenIssuancePolicy](tokenissuancepolicy.md)|As tokenIssuancePolicies atribuídas a essa entidade de serviço.|
|tokenLifetimePolicies|Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)|O tokenLifetimePolicies atribuído a essa entidade de serviço.|

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
  "notes": "string",
  "publishedPermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "passwordSingleSignOnSettings": {"@odata.type": "microsoft.graph.passwordSingleSignOnSettings"},
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
  "useCustomTokenSigningKey": false,
  "verifiedPublisher": {"@odata.type": "microsoft.graph.verifiedPublisher"}
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



