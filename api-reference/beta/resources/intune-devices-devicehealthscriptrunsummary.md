---
title: tipo de recurso deviceHealthScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c3e96083cdbc1c59b9e77d18bbf1b2e1a081ff37
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539075"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a>tipo de recurso deviceHealthScriptRunSummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Leia as propriedades e as relações do objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .|
|[Atualizar deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Atualiza as propriedades de um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de Resumo de execução de script de integridade do dispositivo. Essa propriedade é somente leitura.|
|noIssueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro|
|issueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção encontrou um problema|
|detectionScriptErrorDeviceCount|Int32|Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída|
|detectionScriptPendingDeviceCount|Int32|Número de dispositivos que ainda não executaram a versão mais recente do script de integridade do dispositivo|
|issueRemediatedDeviceCount|Int32|Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado|
|remediationSkippedDeviceCount|Int32|Número de dispositivos para os quais a correção foi ignorada|
|issueReoccurredDeviceCount|Int32|Número de dispositivos para os quais o script de correção foi executado com êxito, mas falhou ao resolver o problema detectado|
|remediationScriptErrorDeviceCount|Int32|Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída|
|lastScriptRunDateTime|DateTimeOffset|Hora da última execução para o script em todos os dispositivos|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```



