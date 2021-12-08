---
title: Ação executeAction
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb4a283d2954e0e37828475635727f3fcd6ffe62
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344649"
---
# <a name="executeaction-action"></a>Ação executeAction

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/executeAction
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
|actionName|[driverApprovalAction](../resources/intune-softwareupdate-driverapprovalaction.md)|Ainda não documentado|
|driverIds|String collection|Ainda não documentado|
|deploymentDate|DateTimeOffset|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [bulkDriverActionResult](../resources/intune-softwareupdate-bulkdriveractionresult.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/executeAction

Content-type: application/json
Content-length: 137

{
  "actionName": "decline",
  "driverIds": [
    "Driver Ids value"
  ],
  "deploymentDate": "2016-12-31T23:58:18.3419405-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": {
    "@odata.type": "microsoft.graph.bulkDriverActionResult",
    "successfulDriverIds": [
      "Successful Driver Ids value"
    ],
    "failedDriverIds": [
      "Failed Driver Ids value"
    ],
    "notFoundDriverIds": [
      "Not Found Driver Ids value"
    ]
  }
}
```




