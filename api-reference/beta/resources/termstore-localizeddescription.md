---
title: Tipo de recurso localizedDescription
description: Representa a descrição localizada usada para descrever um termo no repositório de termos.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 8506bcb39eeb006f6cea45c1f2d0574af0b71c65
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732342"
---
# <a name="localizeddescription-resource-type"></a>Tipo de recurso localizedDescription

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a descrição localizada usada para descrever [um termo] no repositório de [termos].


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|A descrição no idioma localizado.|
|languageTag|String|A marca de idioma do rótulo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedDescription"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedDescription",
  "description": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.term]: termStore-term.md
[microsoft.graph.termStore.store]: termStore-store.md
[Termo]: ../resources/termstore-term.md
[Loja]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription&quot;: &quot;#"
  },
  "suppressions": []
}
-->


