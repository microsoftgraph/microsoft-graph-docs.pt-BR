---
title: Tipo de recurso qualityUpdateReference
description: Representa Windows 10 conteúdo de atualização de qualidade.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ecfddf24b8e2550f55c28ef60e218b5caae985da
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861595"
---
# <a name="qualityupdatereference-resource-type"></a>Tipo de recurso qualityUpdateReference

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa Windows 10 conteúdo de atualização de qualidade.

Em uma implantação, a mesma referência de atualização de qualidade pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.

Herda de [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md). Tipo base [de expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classificação|microsoft.graph.windowsUpdates.qualityUpdateClassification|Especifica a classificação do conteúdo referenciado. Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**. Os valores possíveis são: `security` e `unknownFutureValue`.|
|releaseDateTime|DateTimeOffset|Especifica uma atualização de qualidade no determinado serviçoChannel com a classificação determinada por data (ou seja, a última atualização publicada na data especificada). O valor padrão é `security`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)"
}
```

