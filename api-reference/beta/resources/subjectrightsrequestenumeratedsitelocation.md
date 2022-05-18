---
title: Tipo de recurso subjectRightsRequestEnumeratedSiteLocation
description: Representa as propriedades de uma solicitação de direitos de entidade que define sites específicos (sites SharePoint, sites OneDrive for Business e canais Microsoft Teams assunto) como um local de pesquisa.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b7b8752fb51da3eaaa9762de7b38cf080559a5e4
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461651"
---
# <a name="subjectrightsrequestenumeratedsitelocation-resource-type"></a>Tipo de recurso subjectRightsRequestEnumeratedSiteLocation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as propriedades de uma solicitação de direitos de entidade que define sites específicos (sites SharePoint, sites OneDrive for Business e canais Microsoft Teams assunto) como um local de pesquisa.

Herda de [subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Urls|Coleção de cadeias de caracteres|Conjunto de URLs de site que devem ser incluídas. Inclui a URL de cada site, por exemplo, `https://www.contoso.com/site1`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestEnumeratedSiteLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestEnumeratedSiteLocation",
  "urls": [
    "String"
  ]
}
```

