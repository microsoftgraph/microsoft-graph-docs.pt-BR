---
title: 'channel: doesUserHaveAccess'
description: Determine se um usuário tem acesso a um canal compartilhado.
author: devjha-ms
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 808814a7c535a8a2ba9856eda0d8ec36a1170670
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211036"
---
# <a name="channel-doesuserhaveaccess"></a>channel: doesUserHaveAccess
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Determine se um [usuário](../resources/useridentity.md) tem acesso a um canal [compartilhado](../resources/channel.md).

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante) | ChannelMember.Read.All, ChannelMember.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelMember.Read.All, ChannelMember.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/channels/{channel-id}/doesUserHaveAccess
```

## <a name="function-parameters"></a>Parâmetros de função
Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|tenantId|String|A ID do Azure Active Directory locatário ao [qual o usuário](../resources/useridentity.md) pertence. O valor padrão para essa propriedade é a **tenantId** atual do usuário ou aplicativo conectado.|
|userId|Cadeia de caracteres|Identificador exclusivo do [usuário](../resources/useridentity.md). Especifique **a userId** ou **a propriedade userPrincipalName** na solicitação.|
|userPrincipalName|Cadeia de caracteres|O nome UPN do [usuário](../resources/useridentity.md). Especifique **a userId** ou **a propriedade userPrincipalName** na solicitação.|


## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para essa função.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-check-access-for-an-internal-user"></a>Exemplo 1: Verificar o acesso de um usuário interno

A seguir está um exemplo de uma solicitação que verifica se um usuário interno tem acesso a um canal compartilhado.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userId='6285581g-484b-4845-9e01-60667f8b12ae')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```


### <a name="example-2-check-access-for-an-external-user"></a>Exemplo 2: Verificar o acesso de um usuário externo

Veja a seguir um exemplo de uma solicitação que usa a propriedade **tenantId** para verificar se um usuário externo tem acesso a um canal compartilhado.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess_externaluser"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userId='62855810-484b-4823-9e01-60667f8b12ae', tenantId='57fb72d0-d811-46f4-8947-305e6072eaa5')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-externaluser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-externaluser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-externaluser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-externaluser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```


### <a name="example-3-check-user-access-for-a-user-using-the-user-principal-name"></a>Exemplo 3: Verificar o acesso do usuário para um usuário usando o nome principal do usuário

Veja a seguir um exemplo de uma solicitação que usa a **propriedade userPrincipalName** para verificar se um usuário interno tem acesso a um canal compartilhado.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess_usingupn"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userPrincipalName='john.doe@contoso.com')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-usingupn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-usingupn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-usingupn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-usingupn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": false
}
```

