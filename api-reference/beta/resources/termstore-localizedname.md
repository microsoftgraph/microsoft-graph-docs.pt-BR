---
title: tipo de recurso localizedName
description: Representa o nome localizado usado no repositório de termos, que identifica o nome no idioma localizado.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 3f6308689f1f370e3463b9cc095da211dc612de1
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734233"
---
# <a name="localizedname-resource-type"></a>tipo de recurso localizedName

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome localizado usado no repositório [de termos], que identifica o nome no idioma localizado. Para obter mais informações, [consulte localizedLabel].

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|languageTag|String|A marca de idioma do rótulo.|
|nome|String|O nome no idioma localizado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedName",
  "name": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.localizedLabel]: termstore-localizedlabel.md
[microsoft.graph.termstore.store]: termstore-store.md
[loja]: ../resources/termstore-store.md
[localizedLabel]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName&quot;: &quot;#"
  },
  "suppressions": []
}
-->


