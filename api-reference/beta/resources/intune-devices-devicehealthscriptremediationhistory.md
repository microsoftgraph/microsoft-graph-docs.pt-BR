---
title: Tipo de recurso deviceHealthScriptRemediationHistory
description: O número de dispositivos remediados por um script de saúde do dispositivo em uma determinada data com a última hora modificada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed2abbd5326121cf98f8e9c226ff8dd2e070b1f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58751906"
---
# <a name="devicehealthscriptremediationhistory-resource-type"></a>Tipo de recurso deviceHealthScriptRemediationHistory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O número de dispositivos remediados por um script de saúde do dispositivo em uma determinada data com a última hora modificada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data em que o histórico de resultados é calculado para o healthscript.|
|historyData|[Coleção deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md)|O número de dispositivos remediados pelo script de saúde do dispositivo na data determinada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistory",
  "lastModifiedDateTime": "String (timestamp)",
  "historyData": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
      "date": "String (Date)",
      "remediatedDeviceCount": 1024,
      "noIssueDeviceCount": 1024
    }
  ]
}
```



