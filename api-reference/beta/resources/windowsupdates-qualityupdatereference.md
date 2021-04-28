---
title: Tipo de recurso qualityUpdateReference
description: Representa Windows 10 conteúdo de atualização de qualidade.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ca416ba5031e4642a073f4796ee27996d22f0f5a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067790"
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
|classificação|microsoft.graph.windowsUpdates.qualityUpdateClassification|Especifica a classificação do conteúdo referenciado. Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**. Os valores possíveis são: `security` .|
|releaseDateTime|DateTimeOffset|Especifica uma atualização de qualidade no determinado serviçoChannel com a classificação determinada por data (ou seja, a última atualização publicada na data especificada). O valor padrão é segurança.|

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

