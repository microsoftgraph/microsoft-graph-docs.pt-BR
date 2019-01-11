---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8bce2e359627ede66f32d696c8a84d2ba9faccec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811652"
---
# <a name="mediacontentratingunitedstates-resource-type"></a>Tipo de recurso mediaContentRatingUnitedStates

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|movieRating|[ratingUnitedStatesMoviesType](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|Filmes classificação selecionado para os Estados Unidos. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.|
|tvRating|[ratingUnitedStatesTelevisionType](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|Classificação de TV selecionada para os Estados Unidos. Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```





