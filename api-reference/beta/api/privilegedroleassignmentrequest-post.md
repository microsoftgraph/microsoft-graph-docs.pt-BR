---
title: Criar privilegedRoleAssignmentRequest
description: Crie um objeto privilegedroleassignmentrequest.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: b54785f4c857b3c7c45ffbba3c81e2d64f2a427a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399506"
---
# <a name="create-privilegedroleassignmentrequest"></a>Criar privilegedRoleAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Crie um [objeto privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD    |
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) . 

| Propriedade     | Tipo    |  Descrição|
|:---------------|:--------|:----------|
|roleId|Cadeia de caracteres|A ID da função. Obrigatório.|
|type|Cadeia de caracteres|Representa o tipo da operação na atribuição de função. O valor pode ser: administradores `AdminAdd`adicionam usuários a funções;`UserAdd`: os usuários adicionam atribuições de função. Obrigatório.|
|assignmentState|Cadeia de caracteres|O estado da atribuição. O valor pode ser `Eligible` para `Active` atribuição qualificada - `Active` se ele for atribuído diretamente por administradores ou ativado em uma atribuição qualificada pelos usuários. Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Obrigatório.|
|motivo|Cadeia de caracteres|O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e revisão.|
|Cronograma|[governanceSchedule](../resources/governanceschedule.md)|O agendamento da solicitação de atribuição de função.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.

### <a name="error-codes"></a>Códigos de erro
Essa API retorna os códigos de erro HTTP padrão. Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.

|Código de erro     | Mensagem de erro              | 
|:--------------------| :---------------------|
| 400 BadRequest | A propriedade RoleAssignmentRequest era NULL |
| 400 BadRequest | Não é possível desserializar o objeto roleAssignmentRequest. |
| 400 BadRequest | RoleId é necessário. |
| 400 BadRequest | A data de início da agenda deve ser especificada e deve ser maior que Agora. |
| 400 BadRequest | Já existe uma agenda para esse usuário, função e tipo de agendamento. |
| 400 BadRequest | Já existe uma aprovação pendente para esse usuário, função e tipo de aprovação. |
| 400 BadRequest | O motivo do solicitante está ausente. |
| 400 BadRequest | O motivo do solicitante deve ter menos de 500 caracteres. |
| 400 BadRequest | A duração da elevação deve estar entre 0,5 e {from setting}. |
| 400 BadRequest | Há uma sobreposição entre a ativação agendada e a solicitação. |
| 400 BadRequest | A função já está ativada. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: as informações de tique são necessárias e não são fornecidas no processo de ativação. |
| 400 BadRequest | Há uma sobreposição entre a ativação agendada e a solicitação. |
| 403 Não Autorizado | A elevação requer Autenticação Multifator. |
| 403 Não Autorizado | Em nome da elevação não é permitido. |

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-privilegedroleassignmentrequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-privilegedroleassignmentrequest-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Eis um exemplo da resposta. Observação: o objeto de resposta exibido aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


