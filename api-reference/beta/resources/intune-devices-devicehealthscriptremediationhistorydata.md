---
title: tipo de recurso deviceHealthScriptRemediationHistoryData
description: O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7095dc821ccfaada8d1f83047895f54d823e1958
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060283"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a>tipo de recurso deviceHealthScriptRemediationHistoryData

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O número de dispositivos corrigidos por um script de integridade do dispositivo em uma determinada data.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|data|Data|A data em que os dispositivos foram corrigidos pelo script de integridade do dispositivo.|
|remediatedDeviceCount|Int32|O número de dispositivos corrigidos pelo script de integridade do dispositivo.|
|noIssueDeviceCount|Int32|O número de dispositivos que foram encontrados não têm problema pelo script de integridade do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "String (Date)",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```






