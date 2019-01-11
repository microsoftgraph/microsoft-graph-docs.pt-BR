---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 502abcae283b7e97e04ab2c342e6b526b41f64f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829880"
---
# <a name="mediacontentratingfrance-resource-type"></a>Tipo de recurso mediaContentRatingFrance

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|movieRating|[ratingFranceMoviesType](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|Filmes selecionado de classificação da França. Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.|
|tvRating|[ratingFranceTelevisionType](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|Classificação de TV selecionada para França. Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



