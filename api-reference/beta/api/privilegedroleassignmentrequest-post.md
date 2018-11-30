---
title: Criar privilegedRoleAssignmentRequest
description: Crie um objeto privilegedroleassignmentrequest.
ms.openlocfilehash: e262682b5a5e8bffa7fb089ae783f3bb7e67803c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037067"
---
# <a name="create-privilegedroleassignmentrequest"></a>Criar privilegedRoleAssignmentRequest

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Crie um objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All    |
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
No corpo da solicitação, fornece uma representação JSON do objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) . 

| Propriedade     | Tipo    |  Descrição|
|:---------------|:--------|:----------|
|roleId|String|A identificação da função. Obrigatório.|
|type|String|Representa o o tipo da operação na atribuição de função. O valor pode ser `AdminAdd`: administradores adicionar usuários às funções; `UserAdd`: Os usuários adicionar atribuições de função. Obrigatório.|
|assignmentState|String|O estado da atribuição. O valor pode ser `Eligible` para atribuição elegível `Active` - se ele é atribuído diretamente `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários. Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Obrigatório.|
|motivo|String|O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.|
|agenda|[governanceSchedule](../resources/governanceschedule.md)|O agendamento da solicitação de atribuição de função.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.

### <a name="error-codes"></a>Códigos de erro
Essa API retorna esse padrão códigos de erro HTTP. Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.

|Código de erro     | Mensagem de erro              | 
|:--------------------| :---------------------|
| 400 BadRequest | Propriedade RoleAssignmentRequest foi NULL |
| 400 BadRequest | Não é possível desserializar roleAssignmentRequest objeto. |
| 400 BadRequest | RoleId é necessário. |
| 400 BadRequest | Data de início de agendamento deve ser especificada e deve ser maior do que agora. |
| 400 BadRequest | Já existe um agendamento para esse tipo de usuário, a função e a agenda. |
| 400 BadRequest | Uma aprovação pendente já existe para esse tipo de usuário, função e aprovação. |
| 400 BadRequest | Motivo solicitante está faltando. |
| 400 BadRequest | Motivo solicitante deve ser menor do que 500 caracteres. |
| 400 BadRequest | Duração de elevação deve estar entre 0,5 e {de configuração}. |
| 400 BadRequest | Não há uma sobreposição entre a ativação agendada e a solicitação. |
| 400 BadRequest | A função já está ativada. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: Tickting informações é necessário e não são fornecidas no processo de ativação. |
| 400 BadRequest | Não há uma sobreposição entre a ativação agendada e a solicitação. |
| 403 não autorizado | Elevação exige a autenticação multifator. |
| 403 não autorizado | Em nome de elevação não é permitida. |

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
Este é um exemplo de resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
