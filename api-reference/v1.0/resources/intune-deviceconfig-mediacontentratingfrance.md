---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcc2364f3327d14afaf32bafafdd98638ea46d39c49bad67169d7a6b292f1ab8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218678"
---
# <a name="mediacontentratingfrance-resource-type"></a>Tipo de recurso mediaContentRatingFrance

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|movieRating|[ratingFranceMoviesType](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|Classificação de filmes selecionada para a França. Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.|
|tvRating|[ratingFranceTelevisionType](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|Classificação de TV selecionada para a França. Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.|

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




