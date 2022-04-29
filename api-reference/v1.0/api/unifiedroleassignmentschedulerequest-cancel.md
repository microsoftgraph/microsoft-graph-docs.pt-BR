---
title: 'unifiedRoleAssignmentScheduleRequest: cancel'
description: Cancele imediatamente um objeto unifiedRoleAssignmentScheduleRequest cujo status é Concedido.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4b6adfff2587338b9196a1612e42590115da0582
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133938"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a>unifiedRoleAssignmentScheduleRequest: cancel
Namespace: microsoft.graph

Cancele imediatamente um objeto [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) que esteja em um status e faça com que o sistema exclua automaticamente a `Granted` solicitação cancelada após 30 dias. Depois de chamar essa ação, **o status** do **unifiedRoleAssignmentScheduleRequest** cancelado muda para `Canceled`.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestId}/cancel
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`. A tentativa de cancelar uma solicitação que não está em um estado cancelável, por exemplo, um objeto **unifiedRoleAssignmentScheduleRequest** cujo **status** `Provisioned` é ou `Failed`retorna `400 Bad Request` um código de erro.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequestthis.cancel"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/95c690fb-3eb3-4942-a03f-4524aed6f31e/cancel
```


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

