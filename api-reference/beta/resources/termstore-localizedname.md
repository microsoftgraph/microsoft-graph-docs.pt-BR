---
title: tipo de recurso localizadoname
description: Representa o nome localizado usado no repositório de termos, que identifica o nome no idioma localizado.
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 5c9e6d4cd614c242e8f915fde71eadd07aa5de15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973593"
---
# <a name="localizedname-resource-type"></a>tipo de recurso localizadoname

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome localizado usado no [repositório]de termos, que identifica o nome no idioma localizado. Para obter mais informações, consulte [localizedLabel].

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
    "Resources/termStore.termLocalizedName": "#"
  },
  "suppressions": []
}
-->


