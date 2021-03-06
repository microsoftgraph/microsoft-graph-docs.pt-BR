---
title: Atualizar deviceComplianceScriptRunSummary
description: Atualiza as propriedades de um objeto deviceComplianceScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b9f723b924028a73facdee32073508f1743511a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310864"
---
# <a name="update-devicecompliancescriptrunsummary"></a>Atualizar deviceComplianceScriptRunSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de Resumo de execução de script de conformidade do dispositivo. Essa propriedade é somente leitura.|
|noIssueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro. Valores válidos-2147483648 a 2147483647|
|issueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção encontrou um problema. Valores válidos-2147483648 a 2147483647|
|detectionScriptErrorDeviceCount|Int32|Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída. Valores válidos-2147483648 a 2147483647|
|detectionScriptPendingDeviceCount|Int32|Número de dispositivos que ainda não executaram a versão mais recente do script de conformidade do dispositivo. Valores válidos-2147483648 a 2147483647|
|lastScriptRunDateTime|DateTimeOffset|Hora da última execução para o script em todos os dispositivos|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "dad42f14-2f14-dad4-142f-d4da142fd4da",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```




