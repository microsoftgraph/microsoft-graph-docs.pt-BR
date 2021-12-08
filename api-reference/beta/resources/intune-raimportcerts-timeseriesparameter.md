---
title: Tipo de recurso timeSeriesParameter
description: Parâmetro passado para GetHealthMetricTimeSeries ao solicitar séries de tempo de instantâneo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25af04afe10ffb6ee7acfdb036871f029c7e1539
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336857"
---
# <a name="timeseriesparameter-resource-type"></a>Tipo de recurso timeSeriesParameter

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parâmetro passado para GetHealthMetricTimeSeries ao solicitar séries de tempo de instantâneo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|metricName|String|O nome da métrica para a qual uma série de tempo é solicitada.|
|startDateTime|DateTimeOffset|Hora de início da série que está sendo solicitada.|
|endDateTime|DateTimeOffset|Hora de término da série que está sendo solicitada. Opcional; se não for especificado, a hora atual será usada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.timeSeriesParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeSeriesParameter",
  "metricName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```




