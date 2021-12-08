---
title: Tipo de recurso certificateConnectorHealthMetricValue
description: Valor de instantâneo métrico retornado em resposta a uma solicitação GetHealthMetricTimeSeries.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6201f79b302378d1452284ed52d14dab4eccc94
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341002"
---
# <a name="certificateconnectorhealthmetricvalue-resource-type"></a>Tipo de recurso certificateConnectorHealthMetricValue

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valor de instantâneo métrico retornado em resposta a uma solicitação GetHealthMetricTimeSeries.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dateTime|DateTimeOffset|Timestamp para esse ponto de dados métrico.|
|successCount|Int64|Contagem de solicitações/operações bem-sucedidas.|
|failureCount|Int64|Contagem de solicitações/operações com falha.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorHealthMetricValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorHealthMetricValue",
  "dateTime": "String (timestamp)",
  "successCount": 1024,
  "failureCount": 1024
}
```




