---
title: Atualizar deviceComplianceScriptDeviceState
description: Atualize as propriedades de um objeto deviceComplianceScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d4f61c14eda8d1187acaab07d92975e07710ba5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130774"
---
# <a name="update-devicecompliancescriptdevicestate"></a>Atualizar deviceComplianceScriptDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do dispositivo de script de conformidade do dispositivo. Essa propriedade é somente leitura.|
|detectionState|[runState](../resources/intune-shared-runstate.md)|Estado de detecção da última execução de script de conformidade do dispositivo. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|O último horário de quando o script de conformidade do dispositivo foi executado|
|expectedStateUpdateDateTime|DateTimeOffset|O próximo horário de quando o script de conformidade do dispositivo deve ser executado|
|lastSyncDateTime|DateTimeOffset|A última vez que a Extensão de Managment do Intune foi sincronizada com o Intune|
|scriptOutput|Cadeia de caracteres|Saída do script de detecção|
|scriptError|Cadeia de caracteres|Erro do script de detecção|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 436

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "7bd39c86-9c86-7bd3-869c-d37b869cd37b",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```




