---
title: Tipo de recurso timeSeriesParameter
description: Parâmetro passado para GetHealthMetricTimeSeries ao solicitar séries de tempo de instantâneo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3110404b04bbea136bc242ab52fd87cdb9f502a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080664"
---
# <a name="timeseriesparameter-resource-type"></a>Tipo de recurso timeSeriesParameter

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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



