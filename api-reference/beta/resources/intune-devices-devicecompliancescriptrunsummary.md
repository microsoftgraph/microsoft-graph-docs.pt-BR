---
title: tipo de recurso deviceComplianceScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a53b536ed8958e82b487e2f244d53077e7c21112
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060500"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a>tipo de recurso deviceComplianceScriptRunSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Leia as propriedades e as relações do objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .|
|[Atualizar deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Atualiza as propriedades de um objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de Resumo de execução de script de conformidade do dispositivo. Essa propriedade é somente leitura.|
|noIssueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro. Valores válidos-2147483648 a 2147483647|
|issueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção encontrou um problema. Valores válidos-2147483648 a 2147483647|
|detectionScriptErrorDeviceCount|Int32|Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída. Valores válidos-2147483648 a 2147483647|
|detectionScriptPendingDeviceCount|Int32|Número de dispositivos que ainda não executaram a versão mais recente do script de conformidade do dispositivo. Valores válidos-2147483648 a 2147483647|
|lastScriptRunDateTime|DateTimeOffset|Hora da última execução para o script em todos os dispositivos|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```






