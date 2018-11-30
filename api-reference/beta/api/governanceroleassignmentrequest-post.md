---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função. A tabela a seguir lista as operações.
ms.openlocfilehash: b0d9edab1182d4a6fa620cfb953df1cb8af20c66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036014"
---
# <a name="create-governanceroleassignmentrequest"></a>Criar governanceRoleAssignmentRequest

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função. A tabela a seguir lista as operações.

| Operação       | Tipo | 
|:---------------|:----------|
| Atribuir uma atribuição de função| AdminAdd |
| Ativar uma atribuição de função elegíveis| UserAdd | 
| Desativar uma atribuição de função ativada| UserRemove | 
| Remover uma atribuição de função| AdminRemove |
| Atualizar uma atribuição de função| AdminUpdate |
| Solicitação para estender minha atribuição de função| UserExtend | 
| Estender uma atribuição de função| AdminExtend | 
| Solicitação de renovação minha atribuição de função expirados| UserRenew | 
| Renovar uma atribuição de função expirados| AdminRenew | 

 
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método não **suporte [parâmetros de consulta OData](/graph/query-parameters)** .

### <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | Portador {código}|
| Content-type  | application/json|

### <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) . 

| Propriedade     | Tipo    |Obrigatório|  Descrição|
|:---------------|:--------|:----------|:----------|
|resourceId|Cadeia de caracteres|Sim|A ID do recurso.|
|roleDefinitionId|String|Sim|A ID da definição de função.|
|subjectId|String|Sim|A identificação do assunto.|
|assignmentState|String|Sim|O estado da atribuição. O valor pode ser ``Eligible`` e ``Active``.|
|type|String|Sim|O tipo de solicitação. O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`e `AdminExtend`.|
|motivo|String| |O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.|
|agenda|[governanceSchedule](../resources/governanceschedule.md)| | O agendamento da solicitação de atribuição de função. Tipo de solicitação de `UserAdd`, `AdminAdd`, `AdminUpdate`, e `AdminExtend`, é necessário.|

### <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.

## <a name="error-codes"></a>Códigos de erro
Essa API segue o padrão dos códigos HTTP, além dos códigos de erro listados na tabela a seguir.

|Código de erro     | Mensagem de erro              | Detalhes |
|:--------------------| :---------------------|:--------------------|
| 400 BadRequest | RoleNotFound    | O `roleDefinitionId` fornecida na solicitação de corpo não pode ser encontrado.
| 400 BadRequest | ResourceIsLocked    | O recurso fornecido no corpo da solicitação está em estado de `Locked` e não pode criar solicitações de atribuição de função.
| 400 BadRequest | SubjectNotFound    | O `subjectId` fornecida na solicitação de corpo não pode ser encontrado.
| 400 BadRequest | PendingRoleAssignmentRequest    | Já existe uma pendente [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.
| 400 BadRequest | RoleAssignmentExists    | [GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criada já existe no sistema.
| 400 BadRequest | RoleAssignmentDoesNotExist    | [GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.
| 400 BadRequest | RoleAssignmentRequestPolicyValidationFailed | O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.

## <a name="example-1"></a>Exemplo 1
Neste exemplo, os administradores atribuem nawu@fimdev.net usuário à função Leitor de cobrança.

 >**Observação:** Além de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso. 

| Propriedade     | Tipo    |Obrigatório|  Valor |
|:---------------|:--------|:----------|:----------|
|resourceId|Cadeia de caracteres|Sim|\<resourceId\>|
|roleDefinitionId|String|Sim|\<roleDefinitionId\>|
|subjectId|String|Sim|\<subjectId\>|
|assignmentState|String|Sim| Elegíveis / ativo|
|type|String|Sim| AdminAdd|
|motivo|String| depende de configurações de função||
|agenda|[governanceSchedule](../resources/governanceschedule.md)|Sim|        |
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "",
    "type": "AdminAdd",
    "assignmentState": "Eligible",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:38:34.6007266Z",
    "roleAssignmentEndDateTime": "2018-11-08T23:37:43.356Z",
    "reason": "Evaluate Only",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "AdminRequestRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:37:43.356Z",
        "endDateTime": "2018-11-08T23:37:43.356Z",
        "duration": "PT0S"
    }
}
```

## <a name="example-2"></a>Exemplo 2
Neste exemplo, nawu@fimdev.net o usuário ativa a função de leitor de faturamento elegível.

| Propriedade     | Tipo    |Obrigatório|  Valor |
|:---------------|:--------|:----------|:----------|
|resourceId|Cadeia de caracteres|Sim|\<resourceId\>|
|roleDefinitionId|String|Sim|\<roleDefinitionId\>|
|subjectId|String|Sim|\<subjectId\>|
|assignmentState|String|Sim| Ativo|
|type|String|Sim| UserAdd|
|motivo|String| depende de configurações de função||
|agenda|[governanceSchedule](../resources/governanceschedule.md)|Sim|        |
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:29:29.5123911Z",
    "roleAssignmentEndDateTime": "2018-05-13T08:28:43.537Z",
    "reason": "Activate the owner role",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "EligibilityRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            },
            {
                "key": "JustificationRule",
                "value": "Grant"
            },
            {
                "key": "ActivationDayRule",
                "value": "Grant"
            },
            {
                "key": "ApprovalRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:28:43.537Z",
        "endDateTime": "0001-01-01T00:00:00Z",
        "duration": "PT9H"
    }
}
```

## <a name="example-3"></a>Exemplo 3
Neste exemplo, o nawu@fimdev.net usuário desativa a função de leitor de cobrança ativa.

| Propriedade     | Tipo    |Obrigatório|  Valor |
|:---------------|:--------|:----------|:----------|
|resourceId|Cadeia de caracteres|Sim|\<resourceId\>|
|roleDefinitionId|String|Sim|\<roleDefinitionId\>|
|subjectId|String|Sim|\<subjectId\>|
|assignmentState|String|Sim| Ativo|
|type|String|Sim| UserRemove|
|motivo|String| Não||
|agenda|[governanceSchedule](../resources/governanceschedule.md)|Não|        |
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
    "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
    "type": "UserRemove",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": null,
    "roleAssignmentEndDateTime": null,
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a>Exemplo 4
Neste exemplo, os administradores remover nawu@fimdev.net o usuário da função Leitor de cobrança.

 >**Observação:** Além do escopo de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.
 
| Propriedade     | Tipo    |Obrigatório|  Valor |
|:---------------|:--------|:----------|:----------|
|resourceId|Cadeia de caracteres|Sim|\<resourceId\>|
|roleDefinitionId|String|Sim|\<roleDefinitionId\>|
|subjectId|String|Sim|\<subjectId\>|
|assignmentState|String|Sim| Elegíveis / ativo|
|type|String|Sim| AdminRemove|
|motivo|String| Não||
|agenda|[governanceSchedule](../resources/governanceschedule.md)|Não|        |
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a>Exemplo 5
Neste exemplo, os administradores atualizar a atribuição de função para o usuário de nawu@fimdev.net ao proprietário.

 >**Observação:** Além do escopo de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso. 
| Propriedade     | Tipo    |Obrigatório|  Valor |
|:---------------|:--------|:----------|:----------|
|resourceId|Cadeia de caracteres|Sim|\<resourceId\>|
|roleDefinitionId|String|Sim|\<roleDefinitionId\>|
|subjectId|String|Sim|\<subjectId\>|
|assignmentState|String|Sim| Elegíveis / ativo|
|type|String|Sim| AdminUpdate|
|motivo|String| depende roleSettings||
|agenda|[governanceSchedule](../resources/governanceschedule.md)|Sim|        |
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:50:03.4755896Z",
  "roleAssignmentEndDateTime":"2018-06-05T05:42:31Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a>Exemplo 6
Este exemplo estende a atribuição de função expirar para usuário ANUJCUSER Colaborador do serviço de gerenciamento de API.

 >**Observação:** Além do escopo de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.
 
| Propriedade     | Tipo    |Obrigatório|  Valor |
|:---------------|:--------|:----------|:----------|
|resourceId|Cadeia de caracteres|Sim|\<resourceId\>|
|roleDefinitionId|String|Sim|\<roleDefinitionId\>|
|subjectId|String|Sim|\<subjectId\>|
|assignmentState|String|Sim| Elegíveis / ativo |
|type|String|Sim| AdminExtend|
|motivo|String| depende roleSettings||
|agenda|[governanceSchedule](../resources/governanceschedule.md)|Sim|        |
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:54:09.7221332Z",
  "roleAssignmentEndDateTime":"2018-08-10T23:53:55.327Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
