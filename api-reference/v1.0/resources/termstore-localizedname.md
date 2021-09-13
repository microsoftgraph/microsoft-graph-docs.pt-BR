---
title: tipo de recurso localizedName
description: Representa o nome localizado usado no armazenamento de termos, que identifica o nome no idioma localizado.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: e4ef39aff45906c70195a92dfe6c4cabe87385e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128043"
---
# <a name="localizedname-resource-type"></a>tipo de recurso localizedName

Namespace: microsoft.graph.termStore

Representa o nome localizado usado no armazenamento [de]termos , que identifica o nome no idioma localizado. Para obter mais informações, [consulte localizedLabel].

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|languageTag|Cadeia de caracteres|A marca de idioma do rótulo.|
|nome|Cadeia de caracteres|O nome no idioma localizado.|

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


