---
title: Ação getRequestStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8bde5c5ae770563607d48b23d240f425a82fb472
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347078"
---
# <a name="getrequeststatus-action"></a>Ação getRequestStatus

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/operationApprovalRequests/getRequestStatus
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|entityId|String|Ainda não documentado|
|entityType|String|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, essa ação retornará um código de resposta e `200 OK` uma [operaçãoApprovalRequestEntityStatus](../resources/intune-rbac-operationapprovalrequestentitystatus.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/operationApprovalRequests/getRequestStatus

Content-type: application/json
Content-length: 75

{
  "entityId": "Entity Id value",
  "entityType": "Entity Type value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": {
    "@odata.type": "microsoft.graph.operationApprovalRequestEntityStatus",
    "requestId": "Request Id value",
    "requestExpirationDateTime": "2016-12-31T23:58:57.6373767-08:00",
    "requestStatus": "needsApproval",
    "entityLocked": true
  }
}
```




