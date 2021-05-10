---
title: Atualizar unifiedRoleAssignmentScheduleRequest
description: Atualize as propriedades de um objeto unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 39963100f1c9516c35bf3149acdda9807355339f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299100"
---
# <a name="update-unifiedroleassignmentschedulerequest"></a>Atualizar unifiedRoleAssignmentScheduleRequest
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|PrivilegedAccess.ReadWrite.AzureAD|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)

A tabela a seguir mostra as propriedades que são necessárias ao atualizar [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleRequest. Chave, não anulada, somente leitura.|
|ação|Cadeia de caracteres|Representando o tipo da operação na atribuição de função. O valor pode ser <ul><li>`AdminAdd`: Os administradores atribuem usuários/grupos a funções;</li><li>`UserAdd`: Os usuários ativam atribuições qualificadas;</li><li> `AdminUpdate`: Os administradores alteram as atribuições de função existentes</li><li>`AdminRemove`: Os administradores removem usuários/grupos de funções;<li>`UserRemove`: Os usuários desativam as atribuições ativas;<li>`UserExtend`: Os usuários solicitam estender suas atribuições de expiração;</li><li>`AdminExtend`: Os administradores estendem atribuições expiradas.</li><li>`UserRenew`: Os usuários solicitam a renovação de suas atribuições expiradas;</li><li>`AdminRenew`: Os administradores estendem atribuições expiradas.</li></ul>|
|principalId|Cadeia de caracteres|Objectid da entidade à qual a atribuição está sendo concedida.|
|roleDefinitionId|Cadeia de caracteres|ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|
|directoryScopeId|Cadeia de caracteres|ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|appScopeId|Cadeia de caracteres|ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|isValidationOnly|Booliano|Um booleano que determina se a chamada é uma validação ou uma chamada real. De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|targetScheduleId|Cadeia de caracteres|ID do objeto schedule anexado à atribuição.|
|justification|Cadeia de caracteres|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentschedulerequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
Content-Type: application/json
Content-length: 466

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
```http
HTTP/1.1 204 OK

```

<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```-->

