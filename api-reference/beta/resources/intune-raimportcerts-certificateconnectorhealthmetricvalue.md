---
title: Tipo de recurso certificateConnectorHealthMetricValue
description: Valor de instantâneo métrico retornado em resposta a uma solicitação GetHealthMetricTimeSeries.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 91432e5b732c84ca9b94ffbe3f89934d1ac40416
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788756"
---
# <a name="certificateconnectorhealthmetricvalue-resource-type"></a>Tipo de recurso certificateConnectorHealthMetricValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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



