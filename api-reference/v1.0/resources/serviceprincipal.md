---
title: Tipo de recurso servicePrincipal
description: Representa uma instância de um aplicativo em um diretório. Herda de directoryObject.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 83e8df77e43d0ca6711d574ffeebde175bd49cb8
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788569"
---
# <a name="serviceprincipal-resource-type"></a>Tipo de recurso servicePrincipal

Namespace: microsoft.graph

Representa uma instância de um aplicativo em um diretório. Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/serviceprincipal-delta.md). Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) collection | Recupere uma lista de objetos servicePrincipal. |
|[Criar servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | Cria um novo objeto servicePrincipal. |
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Leia as propriedades e as relações do objeto servicePrincipal.|
|[Atualizar servicePrincipal](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Atualize o objeto servicePrincipal. |
|[Excluir servicePrincipal](../api/serviceprincipal-delete.md) | Nenhum(a) |Exclua o objeto servicePrincipal.|
|[Listar servicePrincipals excluídos](../api/directory-deleteditems-list.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de objetos servicePrincipal excluídos recentemente. |
|[Obter servicePrincipal excluído](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Recupere as propriedades de um objeto servicePrincipal excluído recentemente. |
|[Excluir permanentemente servicePrincipal](../api/directory-deleteditems-delete.md) | Nenhum | Exclua permanentemente um objeto servicePrincipal. |
|[Restaurar servicePrincipal excluído](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | Restaure um objeto servicePrincipal excluído recentemente. |
|[Listar createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| Obtenha uma coleção de objeto createdObject.|
|[Listar ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objeto ownedObject.|
|[Obter delta](../api/serviceprincipal-delta.md)|servicePrincipal collection| Obtenha alterações incrementais para entidades de serviço. |
|**Atribuição de funções do aplicativo**| | |
|[List appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) collection| Obtenha as funções de aplicativo às quais esta entidade de serviço foi atribuída.|
|[Adicionar uma atribuição de função do aplicativo](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Atribuir uma função de aplicativo a essa entidade de serviço.|
|[Remover uma atribuição de função do aplicativo](../api/serviceprincipal-delete-approleassignments.md) | Nenhum(a) | Remover uma atribuição de função de aplicativo dessa entidade de serviço.|
|[Listar appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md) |coleção [appRoleAssignment](approleassignment.md)| Obtenha os usuários, grupos e funções de aplicativo atribuídos a essa entidade de serviço.|
|[Adicionar appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| Atribuir uma função de aplicativo dessa entidade de serviço a um usuário, grupo ou entidade de serviço.|
|[Remover appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md) | Nenhum(a) | Remova uma atribuição de função de aplicativo dessa entidade de serviço de um usuário, grupo ou entidade de serviço.|
|**Certificados e segredos**| | |
|[Adicionar senha](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|Adicione uma senha ou segredo forte a um servicePrincipal.|
|[Adicionar tokenSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md)|[selfSignedCertificate](../resources/selfsignedcertificate.md)| Adicione um certificado auto-assinado à entidade de serviço. Usado principalmente para configurar aplicativos SSO baseados em SAML na [galeria do Azure AD](/azure/active-directory/saas-apps/tutorial-list).
|[Remover senha](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|Remova uma senha ou segredo de um servicePrincipal.|
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
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há associação em uma lista de grupos específica.|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|Coleção de cadeias de caracteres|Verifique se há associação em uma lista de grupo específica, função de diretório ou objetos de unidade administrativa.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Coleção de cadeias de caracteres|Obtenha a lista de grupos dos quais essa entidade de serviço é membro.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection|Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.|
|**Owners**| | |
|[Listar proprietários](../api/serviceprincipal-list-owners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objetos owner.|
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

## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#service-principal-properties).

| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
| accountEnabled |Booliano| `true` se a conta da entidade de serviço estiver habilitada; caso contrário, `false`. oferece suporte `$filter` (`eq`, `ne`, `not`, `in`).|
| addIns | Coleção [addIn](addin.md) | Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online&preserve-view=true) para a funcionalidade "FileHandler". Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando.|
|alternativeNames|Coleção de cadeias de caracteres| Usado para recuperar entidades de serviço por assinatura, identificar grupo de recursos e IDs de recursos completos de [identidades gerenciadas](/azure/active-directory/managed-identities-azure-resources/overview). oferece suporte `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|appDescription|String|A descrição exposta pelo aplicativo associado.|
|appDisplayName|String|O nome de exibição exposto pelo aplicativo associado.|
|appId|Cadeia de caracteres|O identificador exclusivo do aplicativo associado (seu **appId** propriedade). Oferece suporte `$filter` (`eq`, `ne`, `not`, `in`, `startsWith`).|
|applicationTemplateId|String|Identificador exclusivo do applicationTemplate do qual o servicePrincipal foi criado. Somente leitura. Oferece suporte `$filter` (`eq`, `ne`, `NOT`, `startsWith`).|
|appOwnerOrganizationId|Guid|Contém a ID de locatário onde o aplicativo está registrado. Isso é aplicável apenas a entidades de serviço respaldadas por aplicativos. Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`).|
|appRoleAssignmentRequired|Booliano|Especifica se os usuários ou outras entidade de serviço precisam receber uma atribuição de função de aplicativo para essa entidade de serviço antes que os usuários possam entrar ou que os aplicativos possam obter tokens. O valor padrão é `false`. Não anulável. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`). |
|appRoles|Coleção [appRole](approle.md)|As funções expostas pelo aplicativo que essa entidade de serviço representa. Para obter mais informações, confira definição da propriedade **appRoles** na entidade [aplicativo](application.md). Não anulável. |
| deletedDateTime | DateTimeOffset | A data e a hora em que a entidade de serviço foi excluída. Somente leitura. |
| descrição | String | Campo de texto disponível para fornecer uma descrição voltada para o usuário final interno da entidade de serviço. Os portais do usuário final, como [MyApps](/azure/active-directory/user-help/my-apps-portal-end-user-access), exibirão a descrição do aplicativo neste campo. O tamanho máximo permitido é de 1.024 caracteres. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`) e `$search`.|
| disabledByMicrosoftStatus | Cadeia de caracteres | Especifica se a Microsoft desabilitou o aplicativo registrado. Os valores possíveis são: `null`(valor padrão), `NotDisabled` e (os motivos podem incluir atividades suspeitas, abusivas ou mal-intencionadas ou uma violação do `DisabledDueToViolationOfServicesAgreement` Contrato de Serviços Microsoft). <br><br> Suporta `$filter` (`eq`, `ne`, `not`).  |
|displayName|String|O nome de exibição da entidade de serviço. Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$search`e `$orderBy`. |
|homepage|String|Página inicial ou página de aterrissagem do aplicativo.|
|id|String|O identificador exclusivo da entidade de serviço. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. Oferece suporte `$filter` (`eq`, `ne`, `not`, `in`).|
| informações  | [informationalUrl](informationalurl.md) | Informações básicas de perfil do aplicativo adquirido, como marketing, suporte, termos de serviço e URLs de política de privacidade do aplicativo. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, confira [Como adicionar termos de serviço e política de privacidade a aplicativos do Azure AD registrados](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). <br><br>Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`e `eq` em `null` valores).  |
|keyCredentials|[keyCredential](keycredential.md) collection|A coleção de credenciais de chave associadas ao aplicativo. Não anulável. Oferece suporte `$filter`(`eq`, `not`, `ge`, `le`).            |
|loginUrl|String|Especifica a URL na qual o provedor de serviços redireciona o usuário para a autenticação do Azure AD. O Azure AD usa a URL para iniciar o aplicativo do Microsoft 365 ou o Azure AD My Apps. Quando em branco, o Azure AD executa o logon iniciado pelo IdP de aplicativos configurados com o [logon único baseado em SAML](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). O usuário inicia o aplicativo do Microsoft 365, o Azure AD My Apps ou a URL de SSO do Azure AD.|
|logoutUrl|Cadeia de caracteres| Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff OpenId Connect [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.|
|notes|String|Campo de texto disponível para capturar informações sobre a entidade de serviço, normalmente usado para fins operacionais. O tamanho máximo permitido é de 1.024 caracteres.|
|NotificationEmailAddresses|Coleção de cadeias de caracteres|Especifica a lista de endereços de email para os quais o Azure AD envia uma notificação quando o certificado ativo está próximo da data de validade. Isso é apenas para os certificados usados ​​para assinar o token SAML emitido para aplicativos da Galeria do Azure AD.|
|oauth2PermissionScopes|coleção [permissionScope](permissionScope.md)|As permissões delegadas expostas pelo aplicativo. Para obter mais informações, confira a propriedade **oauth2PermissionScopes** na propriedade [api](application.md) da entidade **aplicativo**. Não anulável.|
| passwordCredentials | [passwordCredential](passwordcredential.md) collection|A coleção de credenciais de senha associadas ao aplicativo Não anulável.|
|preferredSingleSignOnMode|cadeia de caracteres|Especifica o modo de logon único configurado para este aplicativo. O Azure AD usa o modo de logon único preferido para iniciar o aplicativo do Microsoft 365 ou o Azure AD My Apps. Os valores com suporte são: `password`, `saml`, `notSupported`, e `oidc`.|
|replyUrls|String collection|URLs para as quais os tokens de usuário são enviados para se conectar com a aplicação associada, ou as URIs redirecionadas para as quais os códigos de autorização OAuth 2.0 e os tokens de acesso são enviados para a aplicação associada. Não pode ser anulado. |
|resourceSpecificApplicationPermissions|Coleção [resourceSpecificPermission](../resources/resourcespecificpermission.md)|As permissões de aplicativo específicas do recurso expostas por este aplicativo. Atualmente, as permissões específicas de recursos só têm suporte para aplicativos [Teams que acessam chats e equipes específicos ](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) usando Microsoft Graph. Somente leitura.|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](samlsinglesignonsettings.md)|A coleção das configurações relacionadas ao logon único do SAML.|
|servicePrincipalNames|Coleção de cadeias de caracteres|Contém a lista de **identificadoresUris**, copiados do [aplicativo](application.md) associado. É possível adicionar valores adicionais aos aplicativos híbridos. Esses valores podem ser usados ​​para identificar as permissões apresentadas por esse aplicativo no Azure AD. Por exemplo,<ul><li>Os aplicativos cliente podem especificar um URI de recurso com base nos valores dessa propriedade para adquirir um token de acesso, que é o URI retornado na declaração "aud".</li></ul><br>O operador é necessário para filtrar expressões nas propriedades multivalorizadas. Não pode ser anulado.<br><br> Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|servicePrincipalType|Cadeia de caracteres|Identifica se a entidade de serviço representa um aplicativo, uma identidade gerenciada ou um aplicativo herdado. Isso é definido pelo Azure AD internamente. A propriedade **servicePrincipalType** pode ser definida para três valores diferentes: <ul><li>__Aplicativo__ - Uma entidade de serviço que representa um aplicativo ou serviço. A propriedade **appId** identifica o registro do aplicativo associado e corresponde a **appId** de um [aplicativo](application.md), possivelmente de um locatário diferente. Se o registro do aplicativo associado estiver ausente, os tokens não serão emitidos para a entidade de serviço.</li><li>__ManagedIdentity__ - Uma entidade de serviço que representa uma [identidade gerenciada](/azure/active-directory/managed-identities-azure-resources/overview). As entidades de serviço que representam identidades gerenciadas podem receber acesso e permissões, mas não podem ser atualizadas ou modificadas diretamente.</li><li>__Herdada__ - Uma entidade de serviço que representa um aplicativo criado antes dos registros do aplicativo ou por meio de experiências herdadas. A entidade de serviço herdada pode ter credenciais, nomes de entidade de serviço, URLs de resposta e outras propriedades que podem ser editadas por um usuário autorizado, mas não tem um registro de aplicativo associado. O valor **appId** não associa a entidade de serviço a um registro de aplicativo. A entidade de serviço só pode ser usada no locatário em que foi criada.</li><li>__SocialIdp__ - Para uso interno. </ul>|
| signInAudience | String | Especifique as contas da Microsoft que têm suporte para o aplicativo atual. Somente leitura.<br><br>Os valores com suporte são:<ul><li>`AzureADMyOrg`: Usuários com uma conta Microsoft corporativa ou de estudante no locatário do Azure AD da minha organização (locatário único)</li><li>`AzureADMultipleOrgs`: Usuários com uma conta Microsoft corporativa ou de estudante em locatário Azure AD de qualquer organização (multi locatário)</li><li>`AzureADandPersonalMicrosoftAccount`: Usuários com uma conta Microsoft pessoal, corporativa ou de estudante no locatário do Azure AD de qualquer organização.</li><li>`PersonalMicrosoftAccount`: Somente os usuários com uma conta Microsoft pessoal.</li></ul> |
|tags|Coleção de cadeias de caracteres| Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar a entidade de serviço. Não anulável.<br><br>Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`). |
| tokenEncryptionKeyId |Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD emite tokens para este aplicativo criptografado usando a chave especificada por essa propriedade. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | Especifica o distribuidor verificado do aplicativo que essa entidade de serviço representa.

## <a name="relationships"></a>Relações
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Atribuições de função de aplicativo para este aplicativo ou serviço, concedidas a usuários, grupos e outras entidades de serviço. Suporta `$expand`.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Atribuição da função do aplicativo para outro aplicativo ou serviço, concedida a essa entidade de serviço. Oferece suporte `$expand`.|
|claimsMappingPolicies|Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)|O claimsMappingPolicies atribuído a essa entidade de serviço. Oferece suporte `$expand`.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório criados por essa entidade de serviço. Somente leitura. Anulável.|
|homeRealmDiscoveryPolicies|Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)|O homeRealmDiscoveryPolicies atribuído a essa entidade de serviço. Oferece suporte `$expand`.|
|memberOf|[directoryObject](directoryobject.md) collection|Funções das quais essa entidade de serviço é membro. Métodos HTTP: OBTER Somente leitura. Anulável. Oferece suporte `$expand`.|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) collection|Concessões de permissão delegadas que autorizam essa entidade de serviço a acessar uma API em nome de um usuário conectado. Somente leitura. Anulável.|
|ownedObjects|[directoryObject](directoryobject.md) collection|Objetos de diretório que pertencem a essa entidade de serviço. Somente leitura. Anulável. Oferece suporte `$expand`.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários dessa servicePrincipal. Os proprietários são um conjunto de usuários não administradores ou servicePrincipal que têm permissão para modificar esse objeto. Somente leitura. Anulável. Suporta o `$expand`.|
|tokenIssuancePolicies|coleção [tokenIssuancePolicy](tokenissuancepolicy.md)|As tokenIssuancePolicies atribuídas a essa entidade de serviço.|
|tokenLifetimePolicies|Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)|O tokenLifetimePolicies atribuído a essa entidade de serviço.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

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
  "alternativeNames": ["String"] ,
  "appDisplayName": "String",
  "appId": "String",
  "appOwnerOrganizationId": "Guid",
  "appRoleAssignmentRequired": true,
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "disabledByMicrosoftStatus": "String",
  "displayName": "String",
  "homepage": "String",
  "id": "String (identifier)",
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "String",
  "notes": "String",
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "replyUrls": ["String"],
  "resourceSpecificApplicationPermissions": [{"@odata.type": "microsoft.graph.resourceSpecificPermission"}],
  "servicePrincipalNames": ["String"],
  "servicePrincipalType": "String",
  "tags": ["String"],
  "tokenEncryptionKeyId": "String",
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