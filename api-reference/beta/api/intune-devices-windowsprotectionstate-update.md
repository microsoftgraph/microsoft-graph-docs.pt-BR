---
title: Atualizar windowsProtectionState
description: Atualize as propriedades de um objeto windowsProtectionState.
author: tfitzmac
ms.openlocfilehash: 8bdbe3d1841eb29f7616edcc5063cd025f282974
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308705"
---
# <a name="update-windowsprotectionstate"></a>Atualizar windowsProtectionState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Accept|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo para o objeto de status de proteção do dispositivo. Este é o id do dispositivo do dispositivo|
|malwareProtectionEnabled|Boolean|Anti-malware está habilitado ou não|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.). Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Boolean|Proteção em tempo real está habilitada ou não?|
|networkInspectionSystemEnabled|Boolean|Sistema de inspeção de rede habilitado ou não?|
|quickScanOverdue|Boolean|Verificação rápida vencidos ou não?|
|fullScanOverdue|Boolean|Completos exame vencido ou não?|
|signatureUpdateOverdue|Boolean|Assinatura desatualizada ou não?|
|rebootRequired|Boolean|Reinicialização necessária ou não?|
|fullScanRequired|Boolean|Verificação completa necessária ou não?|
|engineVersion|String|Versão do mecanismo de proteção de ponto de extremidade atual|
|signatureVersion|String|Versão atual de definições de malware|
|antiMalwareVersion|String|Atual anti-malware versão|
|lastQuickScanDateTime|DateTimeOffset|Última data/hora de verificação rápida|
|lastFullScanDateTime|DateTimeOffset|Última data/hora de verificação rápida|
|lastQuickScanSignatureVersion|String|Última versão de assinatura de verificação rápida|
|lastFullScanSignatureVersion|String|Última versão de assinatura de verificação completa|
|lastReportedDateTime|DateTimeOffset|Tempo de informado último status de integridade do dispositivo|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 804

{
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
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
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
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```





