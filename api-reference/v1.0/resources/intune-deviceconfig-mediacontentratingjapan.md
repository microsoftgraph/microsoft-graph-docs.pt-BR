---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75cddc24ad9a35c9f409e092846eae1b255c8411
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730697"
---
# <a name="mediacontentratingjapan-resource-type"></a>Tipo de recurso mediaContentRatingJapan

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|movieRating|[ratingJapanMoviesType](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|Classificação de filmes selecionada para o Japão. Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.|
|tvRating|[ratingJapanTelevisionType](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|Classificação de TV selecionada para o Japão. Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```





