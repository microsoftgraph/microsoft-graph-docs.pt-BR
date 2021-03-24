---
title: Criar deviceHealthScriptDeviceState
description: Crie um novo objeto deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a115878511d7d0317bc17bc38f88538de503b9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130732"
---
# <a name="create-devicehealthscriptdevicestate"></a>Criar deviceHealthScriptDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto deviceHealthScriptDeviceState.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptDeviceState.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do dispositivo de script de saúde do dispositivo. Essa propriedade é somente leitura.|
|detectionState|[runState](../resources/intune-shared-runstate.md)|Estado de detecção da última execução de script de saúde do dispositivo. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|O último período de data/hora de quando o script de saúde do dispositivo foi executado|
|expectedStateUpdateDateTime|DateTimeOffset|O próximo horário de quando o script de saúde do dispositivo deve ser executado|
|lastSyncDateTime|DateTimeOffset|A última vez que a Extensão de Managment do Intune foi sincronizada com o Intune|
|preRemediationDetectionScriptOutput|Cadeia de caracteres|Saída do script de detecção antes da correção|
|preRemediationDetectionScriptError|Cadeia de caracteres|Erro do script de detecção antes da correção|
|remediationScriptError|Cadeia de caracteres|Saída de erro do script de correção|
|postRemediationDetectionScriptOutput|Cadeia de caracteres|Saída de script de detecção após correção|
|postRemediationDetectionScriptError|Cadeia de caracteres|Erro do script de detecção após a correção|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|Estado de correção da última execução do script de saúde do dispositivo. Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
Content-type: application/json
Content-length: 762

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 811

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```




