---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e53e0c0b4edba1616f91fe841e2171010af9a8c2ea462f02e44d464137b3746
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130209"
---
# <a name="mediacontentratingaustralia-resource-type"></a>Tipo de recurso mediaContentRatingAustralia

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|movieRating|[ratingAustraliaMoviesType](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|Classificação de filmes selecionada para a Austrália. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.|
|tvRating|[ratingAustraliaTelevisionType](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|Classificação de TV selecionada para a Austrália. Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




