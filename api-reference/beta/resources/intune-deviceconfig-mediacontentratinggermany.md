---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: b7e02226ccea817a609d6e7f3059bff8e6bdb9ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318358"
---
# <a name="mediacontentratinggermany-resource-type"></a>Tipo de recurso mediaContentRatingGermany

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|movieRating|[ratingGermanyMoviesType](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|Filmes classificação selecionado para a Alemanha. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.|
|tvRating|[ratingGermanyTelevisionType](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|Classificação de TV selecionada para a Alemanha. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```





