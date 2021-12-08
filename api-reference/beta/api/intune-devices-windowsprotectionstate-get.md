---
title: Obter windowsProtectionState
description: Leia propriedades e relações do objeto windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c40ea10792a6f84fc0c67dab42a3749abc2b0f71
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344972"
---
# <a name="get-windowsprotectionstate"></a>Obter windowsProtectionState

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Leia propriedades e relações do [objeto windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1083

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
    "malwareProtectionEnabled": true,
    "deviceState": "fullScanPending",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": true,
    "fullScanOverdue": true,
    "signatureUpdateOverdue": true,
    "rebootRequired": true,
    "fullScanRequired": true,
    "engineVersion": "Engine Version value",
    "signatureVersion": "Signature Version value",
    "antiMalwareVersion": "Anti Malware Version value",
    "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
    "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
    "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
    "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "productStatus": "serviceNotRunning",
    "isVirtualMachine": true,
    "tamperProtectionEnabled": true
  }
}
```




