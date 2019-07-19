---
title: Listar deviceManagementScriptDeviceStates
description: Listar Propriedades e relações dos objetos deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc9349837f12036b9d908aed7a219292c37a3456
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958932"
---
# <a name="list-devicemanagementscriptdevicestates"></a>Listar deviceManagementScriptDeviceStates

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar Propriedades e relações dos objetos [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value"
    }
  ]
}
```





