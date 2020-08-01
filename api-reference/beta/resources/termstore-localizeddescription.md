---
title: tipo de recurso localizedDescription
description: Representa a descrição localizada usada para descrever um termo no repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0bded2c1ad4804fb952ecfd9c75c87f3a8624c7e
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539128"
---
# <a name="localizeddescription-resource-type"></a>tipo de recurso localizedDescription

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a descrição localizada usada para descrever um [termo] no [repositório]de termos.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|A descrição no idioma localizado.|
|languageTag|Cadeia de Caracteres|A marca de idioma do rótulo.|

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
[terminal]: ../resources/termstore-term.md
[Guarde]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription": "#"
  },
  "suppressions": []
}
-->
