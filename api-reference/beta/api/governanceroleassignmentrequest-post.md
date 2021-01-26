---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 19ca4988977807f410a2525110b1b3479d6ea326
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983402"
---
# <a name="create-governanceroleassignmentrequest"></a>Criar governanceRoleAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função. A tabela a seguir lista as operações.

| Operação                                   | Tipo        |
|:--------------------------------------------|:------------|
| Atribuir uma atribuição de função                    | AdminAdd    |
| Ativar uma atribuição de função qualificada        | UserAdd     |
| Desativar uma atribuição de função ativada     | UserRemove  |
| Remover uma atribuição de função                    | AdminRemove |
| Atualizar uma atribuição de função                    | AdminUpdate |
| Solicitação para estender minha atribuição de função        | UserExtend  |
| Estender uma atribuição de função                    | AdminExtend |
| Solicitação para renovar minha atribuição de função expirada | UserRenew   |
| Renovar uma atribuição de função expirada            | AdminRenew  |

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).

### <a name="azure-resources"></a>Recursos do Azure

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

### <a name="azure-ad"></a>Azure Active Directory

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

### <a name="groups"></a>Grupos

|Tipo de permissão | Permissões |
|:-------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureADGroups |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição      |
|:--------------|:-----------------|
| Authorization | Portador {código}    |
| Content-type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)

| Propriedade         | Tipo                                                     | Descrição |
|:-----------------|:---------------------------------------------------------|:--|
| resourceId       | Cadeia de caracteres                                                   | A ID do recurso. Obrigatório. |
| roleDefinitionId | Cadeia de caracteres                                                   | A ID da definição de função. Obrigatório. |
| subjectId        | Cadeia de caracteres                                                   | A ID do assunto. Obrigatório. |
| assignmentState  | Cadeia de caracteres                                                   | O estado da atribuição. O valor pode ser `Eligible` e `Active` . Obrigatório. |
| type             | Cadeia de caracteres                                                   | O tipo de solicitação. O valor pode `AdminAdd` ser , , , , e `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` `AdminExtend` . Obrigatório. |
| motivo           | Cadeia de caracteres                                                   | O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e revisão. |
| Cronograma         | [governanceSchedule](../resources/governanceschedule.md) | O agendamento da solicitação de atribuição de função. Para o tipo de `UserAdd` `AdminAdd` solicitação `AdminUpdate` de , e , `AdminExtend` é necessário. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.

### <a name="error-codes"></a>Códigos de erro

Essa API retorna os códigos de erro HTTP padrão. Além disso, ele também retorna os códigos de erro listados na tabela a seguir.

| Código de erro     | Mensagem de erro                               | Detalhes       |
|:---------------|:--------------------------------------------|:--------------|
| 400 BadRequest | RoleNotFound                                | O `roleDefinitionId` fornecido no corpo da solicitação não pode ser encontrado. |
| 400 BadRequest | ResourceIsLocked                            | O recurso fornecido no corpo da solicitação está no estado e não pode criar `Locked` solicitações de atribuição de função. |
| 400 BadRequest | SubjectNotFound                             | O `subjectId` fornecido no corpo da solicitação não pode ser encontrado. |
| 400 BadRequest | PendingRoleAssignmentRequest                | Já existe uma [governança pendenteRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema. |
| 400 BadRequest | RoleAssignmentExists                        | O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema. |
| 400 BadRequest | RoleAssignmentDoesNotExist                  | O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema. |
| 400 BadRequest | RoleAssignmentRequestPolicyValidationFailed | O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não está de acordo com as políticas internas e não pode ser criado. |

## <a name="examples"></a>Exemplos

Os exemplos a seguir mostram como usar essa API.

### <a name="example-1-administrator-assigns-user-to-a-role"></a>Exemplo 1: O administrador atribui um usuário a uma função

Neste exemplo, um administrador atribui o usuário nawu@contoso.com à função Leitor de Cobrança.

 >**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.

| Propriedade         | Tipo                                                     | Obrigatório                 | Valor |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | Cadeia de caracteres                                                   | Sim                      | \<resourceId\> |
| roleDefinitionId | Cadeia de caracteres                                                   | Sim                      | \<roleDefinitionId\> |
| subjectId        | Cadeia de caracteres                                                   | Sim                      | \<subjectId\> |
| assignmentState  | Cadeia de caracteres                                                   | Sim                      | Qualificado/Ativo |
| type             | Cadeia de caracteres                                                   | Sim                      | AdminAdd |
| motivo           | Cadeia de caracteres                                                   | depende das configurações de função |   |
| Cronograma         | [governanceSchedule](../resources/governanceschedule.md) | Sim                      |   |

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-2-user-activates-eligible-role"></a>Exemplo 2: o usuário ativa a função qualificada

Neste exemplo, o usuário nawu@contoso.com ativa a função leitor de cobrança qualificada.

| Propriedade         | Tipo                                                     | Obrigatório                 | Valor |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | Cadeia de caracteres                                                   | Sim                      | \<resourceId\> |
| roleDefinitionId | Cadeia de caracteres                                                   | Sim                      | \<roleDefinitionId\> |
| subjectId        | Cadeia de caracteres                                                   | Sim                      | \<subjectId\> |
| assignmentState  | Cadeia de caracteres                                                   | Sim                      | Ativo |
| type             | Cadeia de caracteres                                                   | Sim                      | UserAdd |
| motivo           | Cadeia de caracteres                                                   | depende das configurações de função |   |
| Cronograma         | [governanceSchedule](../resources/governanceschedule.md) | Sim                      |   |

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
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

### <a name="example-3-user-deactivates-an-assigned-role"></a>Exemplo 3: o usuário desativa uma função atribuída

Neste exemplo, o usuário nawu@contoso.com desativa a função de Leitor de Cobrança ativa.

| Propriedade         | Tipo                                                     | Obrigatório | Valor |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | Cadeia de caracteres                                                   | Sim      | \<resourceId\> |
| roleDefinitionId | Cadeia de caracteres                                                   | Sim      | \<roleDefinitionId\> |
| subjectId        | Cadeia de caracteres                                                   | Sim      | \<subjectId\> |
| assignmentState  | Cadeia de caracteres                                                   | Sim      | Ativo |
| type             | Cadeia de caracteres                                                   | Sim      | UserRemove |
| motivo           | Cadeia de caracteres                                                   | Não       |   |
| Cronograma         | [governanceSchedule](../resources/governanceschedule.md) | Não       |   |

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "reason": "Evaluate only",
  "schedule": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  }
}
```

### <a name="example-4-administrator-removes-user-from-a-role"></a>Exemplo 4: O administrador remove o usuário de uma função

Neste exemplo, um administrador remove o usuário nawu@contoso.com da função Leitor de Cobrança.

 >**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.

| Propriedade         | Tipo                                                     | Obrigatório | Valor |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | Cadeia de caracteres                                                   | Sim      | \<resourceId\> |
| roleDefinitionId | Cadeia de caracteres                                                   | Sim      | \<roleDefinitionId\> |
| subjectId        | Cadeia de caracteres                                                   | Sim      | \<subjectId\> |
| assignmentState  | Cadeia de caracteres                                                   | Sim      | Qualificado/Ativo |
| type             | Cadeia de caracteres                                                   | Sim      | AdminRemove |
| motivo           | Cadeia de caracteres                                                   | Não       |   |
| Cronograma         | [governanceSchedule](../resources/governanceschedule.md) | Não       |   |

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a>Exemplo 5: O administrador atualiza a atribuição de função

Neste exemplo, os administradores atualizam a atribuição de função do usuário nawu@contoso.com para Proprietário.

 >**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.

| Propriedade         | Tipo                                                     | Obrigatório                | Valor |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | Cadeia de caracteres                                                   | Sim                     | \<resourceId\> |
| roleDefinitionId | Cadeia de caracteres                                                   | Sim                     | \<roleDefinitionId\> |
| subjectId        | Cadeia de caracteres                                                   | Sim                     | \<subjectId\> |
| assignmentState  | Cadeia de caracteres                                                   | Sim                     | Qualificado/Ativo |
| type             | Cadeia de caracteres                                                   | Sim                     | AdminUpdate |
| motivo           | Cadeia de caracteres                                                   | depende de roleSettings |   |
| Cronograma         | [governanceSchedule](../resources/governanceschedule.md) | Sim                     |   |

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
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
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a>Exemplo 6: O administrador estende a atribuição de função expirada

Este exemplo estende a atribuição de função expirada para o usuário ANUJCUSER para o Colaborador do Serviço de Gerenciamento de API.

 >**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.

| Propriedade         | Tipo                                                     | Obrigatório                | Valor |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | Cadeia de caracteres                                                   | Sim                     | \<resourceId\> |
| roleDefinitionId | Cadeia de caracteres                                                   | Sim                     | \<roleDefinitionId\> |
| subjectId        | Cadeia de caracteres                                                   | Sim                     | \<subjectId\> |
| assignmentState  | Cadeia de caracteres                                                   | Sim                     | Qualificado/Ativo |
| type             | Cadeia de caracteres                                                   | Sim                     | AdminExtend |
| motivo           | Cadeia de caracteres                                                   | depende de roleSettings |   |
| Cronograma         | [governanceSchedule](../resources/governanceschedule.md) | Sim                     |   |

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
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
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


