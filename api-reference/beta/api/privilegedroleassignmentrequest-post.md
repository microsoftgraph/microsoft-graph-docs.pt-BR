---
title: Criar privilegedRoleAssignmentRequest
description: Criar um objeto privilegedroleassignmentrequest.
localization_priority: Normal
ms.openlocfilehash: f120181144bc73d7a66c42d03e8743bbbc736582
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337207"
---
# <a name="create-privilegedroleassignmentrequest"></a>Criar privilegedRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
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
No corpo da solicitação, forneça uma representação JSON do objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) . 

| Propriedade     | Tipo    |  Descrição|
|:---------------|:--------|:----------|
|roleId|String|A ID da função. Obrigatório.|
|type|String|Representa o tipo da operação na atribuição de função. O valor pode ser `AdminAdd`: os administradores adicionam usuários a funções; `UserAdd`: Os usuários adicionam atribuições de função. Obrigatório.|
|assignmentstate|String|O estado da atribuição. O valor pode ser `Eligible` para atribuição `Active` qualificada-se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários. Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Obrigatório.|
|motivos|String|O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.|
|futebol|[governanceSchedule](../resources/governanceschedule.md)|O agendamento da solicitação de atribuição de função.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.

### <a name="error-codes"></a>Códigos de erro
Essa API retorna os códigos de erro HTTP padrão. Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.

|Código de erro     | Mensagem de erro              | 
|:--------------------| :---------------------|
| 400 BadRequest | Propriedade RoleAssignmentRequest era nula |
| 400 BadRequest | Não é possível desserializar o objeto roleAssignmentRequest. |
| 400 BadRequest | RoleID é necessário. |
| 400 BadRequest | A data de início agendada deve ser especificada e deve ser maior do que agora. |
| 400 BadRequest | Já existe um cronograma para este usuário, função e tipo de agendamento. |
| 400 BadRequest | Já existe uma aprovação pendente para este usuário, função e tipo de aprovação. |
| 400 BadRequest | Razão do solicitante ausente. |
| 400 BadRequest | O motivo do solicitante deve ser menor que 500 caracteres. |
| 400 BadRequest | A duração da elevação deve estar entre 0,5 e {from Setting}. |
| 400 BadRequest | Há uma sobreposição entre ativação agendada e a solicitação. |
| 400 BadRequest | A função já está ativada. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: as informações de Tickting são necessárias e não são fornecidas no processo de ativação. |
| 400 BadRequest | Há uma sobreposição entre ativação agendada e a solicitação. |
| 403 não autorizado | A elevação requer autenticação multiFator. |
| 403 não autorizado | Em nome da elevação não é permitida. |

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
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
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
##### <a name="response"></a>Resposta
Este é um exemplo de resposta. Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "evaluateOnly": false,
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
  "suppressions": []
}
-->
