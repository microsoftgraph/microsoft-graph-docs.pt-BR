---
title: Atualização de privilegedRoleSettings
description: Atualize as configurações de função para a configuração de função fornecida. Um objeto privilegedRoleSettings será retornado.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 210d70c4ddb7b55003f2e78d9bfcc4e3f64491f6
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399387"
---
# <a name="update-privilegedrolesettings"></a>Atualização de privilegedRoleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as configurações de função para a configuração de função fornecida. Um [objeto privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.
## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Nota:** O solicitante deve ter a função administrador de função com privilégios para atualizar as configurações de função. 

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um [objeto privilegedRoleSettings](../resources/privilegedrolesettings.md) .

A tabela a seguir lista as propriedades que você pode fornecer ao atualizar uma configuração de função.

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|elevationDuration|duração|A duração quando a função é ativada. Obrigatório.|
|id|string|O identificador exclusivo para as configurações de função. Somente leitura. Obrigatório.|
|isMfaOnElevationConfigurable|booliano|**true** se mfaOnElevation for configurável. **false** se mfaOnElevation não for configurável. Obrigatório.|
|lastGlobalAdmin|Booliano|Apenas para uso interno.|
|maxElavationDuration|duração|Duração máxima para a função ativada. Obrigatório.|
|mfaOnElevation|Booliano|**true** se a MFA for necessária para ativar a função. **false** se a MFA não for necessária para ativar a função. Obrigatório.|
|minElevationDuration|duração|Duração mínima para a função ativada. Obrigatório.|
|notificationToUserOnElevation|Booliano|**true** se enviar notificação ao usuário final quando a função for ativada. **false** se não enviar notificação quando a função for ativada. Obrigatório.|
|ticketingInfoOnElevation|Booliano|**true** se as informações de tíquetes são necessárias ao ativar a função. **false** se as informações de tíquete não forem necessárias ao ativar a função. Obrigatório.|
|approvalOnElevation|Booliano|**true** se a aprovação for necessária ao ativar a função. **false** se a aprovação não for necessária ao ativar a função. Obrigatório.|
|approverIds|coleção de cadeias de caracteres|Lista de IDs de aprovação, se a aprovação for necessária para ativação.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Observe que o locatário precisa ser registrado no PIM. Caso contrário, o código de status HTTP 403 Proibido será retornado.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/put-privilegedrolesettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


