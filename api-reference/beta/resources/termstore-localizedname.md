---
title: tipo de recurso localizadoname
description: Representa o nome localizado usado no repositório de termos, que identifica o nome no idioma localizado.
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: cc29deb6e6db5f5664e6fb6bed69195b7183e026
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539127"
---
# <a name="localizedname-resource-type"></a>tipo de recurso localizadoname

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome localizado usado no [repositório]de termos, que identifica o nome no idioma localizado. Para obter mais informações, consulte [localizedLabel].

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|languageTag|Cadeia de Caracteres|A marca de idioma do rótulo.|
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
[Guarde]: ../resources/termstore-store.md
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
