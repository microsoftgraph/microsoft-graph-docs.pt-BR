---
title: Atualizar o servicePrincipalName
description: Atualiza as propriedades do objeto servicePrincipalName.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4a80b28cb42a3c23902fed139f7ccc7ec92ea794
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896130"
---
# <a name="update-serviceprincipal"></a>Atualizar o servicePrincipalName

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades do objeto [servicePrincipalName](../resources/serviceprincipal.md) .

> [!IMPORTANT]
> Não há suporte para o uso de PATCH para definir [**passwordCredential**](../resources/passwordcredential.md) . Use os métodos [addpassword](./serviceprincipal-addpassword.md) e [removePassword](./serviceprincipal-removepassword.md) para atualizar a senha de um servicePrincipalName.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| **True** se a entidade de serviço estiver habilitada; caso contrário, **false**.|
| addIns | [addIn](../resources/addin.md) | Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler". Isso permitirá que os serviços, como o Microsoft 365, chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando.|
|alternativos|Coleção de cadeias de caracteres| Usado para recuperar entidades de serviço por assinatura, identificar grupo de recursos e IDs de recursos completos para [identidades gerenciadas](https://aka.ms/azuremanagedidentity).|
|appRoleAssignmentRequired|Boolean|Especifica se um **appRoleAssignment** de um usuário ou grupo é necessário antes que o Azure AD emita um token de usuário ou de acesso ao aplicativo. Não anulável. |
|appRoles|[appRole](../resources/approle.md) collection|As funções do aplicativo expostas pelo aplicativo associado. Para obter mais informações, consulte a definição da propriedade **appRoles** no recurso [Application](../resources/application.md) . Não anulável. |
|displayName|Cadeia de caracteres|O nome de exibição da entidade de serviço.|
|homepage|String|Página inicial ou página de aterrissagem do aplicativo.|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|A coleção de credenciais principais associada à entidade de serviço. Não anulável.            |
|loginUrl|String|Especifica a URL na qual o provedor de serviços redireciona o usuário para o Azure AD autenticar. O Azure AD usa a URL para iniciar o aplicativo do Microsoft 365 ou do Azure AD meus aplicativos. Quando estiver em branco, o Azure AD executará o logon iniciado pelo IdP para aplicativos configurados com o [logon único baseado em SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). O usuário inicia o aplicativo do Microsoft 365, do Azure AD meus aplicativos ou da URL de SSO do Azure AD.|
|logoutUrl|String| Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.|
|notificationEmailAddresses|Coleção de cadeias de caracteres|Especifica a lista de endereços de email onde o Azure AD envia uma notificação quando o certificado ativo está próximo da data de vencimento. Isso se aplica apenas aos certificados usados para assinar o token SAML emitido para aplicativos da galeria do Azure AD.|
|publishedPermissionScopes|coleção [permissionScope](../resources/permissionScope.md)|As permissões OAuth 2.0 expostas pelo aplicativo associado. Para obter mais informações, consulte a definição da propriedade **oauth2PermissionScopes** no recurso [Application](../resources/application.md) . Não anulável.            |
|preferredSingleSignOnMode|string|Especifica o modo de logon único configurado para este aplicativo. O Azure AD usa o modo de logon único preferencial para iniciar o aplicativo do Microsoft 365 ou do Azure AD meus aplicativos. Os valores com suporte são password, SAML, external e oidc.|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|Especifica a data de expiração da keycredential usada para assinatura de token, marcada por **preferredTokenSigningKeyThumbprint**.|
|preferredTokenSigningKeyThumbprint|String|Reservado apenas para uso interno. Não escreva ou dependa de alguma forma dessa propriedade. Pode ser removida em versões futuras. |
|publisherName|String|O nome de exibição do locatário no qual o aplicativo associado está especificado.|
|replyUrls|String collection|As URLs às quais os tokens de usuário são enviados para entrar com aplicativo associado ou os URIs de redirecionamento aos quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado. Não anulável. |
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)|A coleção para configurações relacionadas ao logon único do SAML.|
|servicePrincipalNames|String collection|Contém a lista de **identifiersUris**, copiadas do [aplicativo](../resources/application.md)associado. Valores adicionais podem ser adicionados aos aplicativos híbridos. Esses valores podem ser usados para identificar as permissões expostas por este aplicativo no Azure AD. Por exemplo,<ul><li>Os aplicativos cliente que solicitam permissões para esse recurso podem usar esses URIs para especificar as permissões necessárias na propriedade **requiredResourceAccess** do manifesto do aplicativo ou na lâmina "permissões de API" na experiência de registro de aplicativos.</li><li>Os aplicativos cliente podem especificar um URI de recurso que se baseia nos valores dessa propriedade para adquirir um token de acesso, que é o URI retornado na declaração "AUD".</li></ul><br>O operador any é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável.|
|tags|String collection| Não anulável. |
|tokenEncryptionKeyId|Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD emite tokens para esse aplicativo criptografado usando a chave especificada por essa propriedade. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `204 No Content` código de resposta e um objeto [servicePrincipalName](../resources/serviceprincipal.md) atualizado no corpo da resposta.
## <a name="examples"></a>Exemplos
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
