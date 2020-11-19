---
title: Listar deviceHealthScripts
description: Listar Propriedades e relações dos objetos deviceHealthScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e80ad3290796b0f4fe5627255fc96f3cf199e918
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49225835"
---
# <a name="list-devicehealthscripts"></a>Listar deviceHealthScripts

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar Propriedades e relações dos objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1578

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScript",
      "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
      "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "runAs32Bit": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "isGlobalScript": true,
      "highestAvailableVersion": "Highest Available Version value",
      "detectionScriptParameters": [
        {
          "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
          "name": "Name value",
          "description": "Description value",
          "isRequired": true,
          "applyDefaultValueWhenNotAssigned": true,
          "defaultValue": "Default Value value"
        }
      ],
      "remediationScriptParameters": [
        {
          "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
          "name": "Name value",
          "description": "Description value",
          "isRequired": true,
          "applyDefaultValueWhenNotAssigned": true,
          "defaultValue": "Default Value value"
        }
      ]
    }
  ]
}
```




