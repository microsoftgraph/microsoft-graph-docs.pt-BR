---
title: Listar raProfileDatabaseEntities
description: Listar Propriedades e relações dos objetos raProfileDatabaseEntity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca8a822b0a79d1e9144261b6cd2f219ee01cbcbb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124175"
---
# <a name="list-raprofiledatabaseentities"></a>Listar raProfileDatabaseEntities

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar Propriedades e relações dos objetos [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .

## <a name="prerequisites"></a>Pré-requisitos
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities
```

### <a name="response"></a>Resposta
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 908

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
      "version": 7,
      "isDeleted": true,
      "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
      "displayName": "Display Name value",
      "linkedProfileIds": [
        "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
      ],
      "profileTypeName": "Profile Type Name value",
      "profileBody": "Profile Body value",
      "profileBodyHash": "Profile Body Hash value",
      "platformType": 12,
      "transformedProfileBody": "Transformed Profile Body value",
      "transformedProfileBodyHash": "Transformed Profile Body Hash value",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "profileId": "6389d896-d896-6389-96d8-896396d88963",
      "eTag": "ETag value",
      "schemaVersion": "betaStart",
      "lastModified": "2017-01-01T00:03:14.6651031-08:00"
    }
  ]
}
```



