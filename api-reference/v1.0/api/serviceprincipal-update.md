---
title: Atualizar serviceprincipal
description: Atualizar as propriedades do objeto serviceprincipal.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a2fe9f45e5d758f8e23b6025d6fddfd9eb62a17f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132009"
---
# <a name="update-serviceprincipal"></a>Atualizar servicePrincipal

Namespace: microsoft.graph

Atualizar as propriedades do objeto [servicePrincipal](../resources/serviceprincipal.md).

> [!IMPORTANT]
> Não há suporte para o uso do PATCH para definir [**passwordCredential**](../resources/passwordcredential.md). Use os métodos [addPassword](./serviceprincipal-addpassword.md) e [removePassword](./serviceprincipal-removepassword.md) para atualizá-la para uma entidade de segurança.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Application.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

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
|accountEnabled|Boolean| **True** se a entidade de serviço estiver habilitada; caso contrário, **false**.|
|addIns| [addIn](../resources/addin.md) | Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos. Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler". Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando.|
|alternativeNames|Coleção de cadeias de caracteres| Usado para recuperar entidades de serviço por assinatura, identificar grupo de recursos e IDs de recursos completos de [identidades gerenciadas](/azure/active-directory/managed-identities-azure-resources/overview).|
|appRoleAssignmentRequired|Boolean|Especifica se um **appRoleAssignment** de um usuário ou grupo é necessário antes que o Azure AD emita um token de usuário ou de acesso ao aplicativo. Não anulável. |
|appRoles|[appRole](../resources/approle.md) collection|As funções do aplicativo expostas pelo aplicativo associado. Para obter mais informações, confira a definição da propriedade **appRoles** no recurso [aplicativo](../resources/application.md). Não anulável. |
|displayName|String|O nome de exibição da entidade de serviço.|
|homepage|Cadeia de caracteres|Página inicial ou página de aterrissagem do aplicativo.|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|A coleta de principais credenciais associadas ao diretor de serviços. Não pode ser anulado.            |
|logoutUrl|String| Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.|
|oauth2PermissionScopes|coleção [permissionScope](../resources/permissionScope.md)|As permissões do escopo OAuth 2.0 expostas pelo aplicativo associado. Para obter mais informações, confira a definição da propriedade **oauth2PermissionScopes** no recurso [aplicativo](../resources/application.md). Não anulável.|
|preferredSingleSignOnMode|cadeia de caracteres|Especifica o modo de logon único configurado para este aplicativo. O Azure AD usa o modo de logon único preferido para iniciar o aplicativo do Microsoft 365 ou o Azure AD My Apps. Os valores com suporte são: `password`, `saml`, `external`, e `oidc`.|
|replyUrls|String collection|URLs para as quais os tokens de usuário são enviados para se conectar com a aplicação associada, ou as URIs redirecionadas para as quais os códigos de autorização OAuth 2.0 e os tokens de acesso são enviados para a aplicação associada. Não pode ser anulado. |
|servicePrincipalNames|Coleção de cadeias de caracteres|Contém a lista de **identificadoresUris**, copiados do [aplicativo](../resources/application.md) associado. É possível adicionar valores adicionais aos aplicativos híbridos. Esses valores podem ser usados ​​para identificar as permissões apresentadas por esse aplicativo no Azure AD. Por exemplo,<ul><li>Os aplicativos cliente solicitando permissões para este recurso podem usar esses URIs para especificar as permissões necessárias na propriedade **requiredResourceAccess** do manifesto do aplicativo, ou na lâmina "permissões de API" na experiência de registros de aplicativos.</li><li>Os aplicativos cliente podem especificar um URI de recurso com base nos valores dessa propriedade para adquirir um token de acesso, que é o URI retornado na declaração "aud".</li></ul><br>O operador é necessário para filtrar expressões nas propriedades multivalorizadas. Não pode ser anulado.|
|tags|Coleção String| Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulada. |
| tokenEncryptionKeyId |Cadeia de caracteres|Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD emite tokens para este aplicativo criptografado usando a chave especificada por essa propriedade. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto atualizado [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/{id}
Content-type: application/json

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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-serviceprincipal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-serviceprincipal-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response"
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