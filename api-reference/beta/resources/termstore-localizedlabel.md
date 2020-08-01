---
title: tipo de recurso localizedLabel
description: Representa o rótulo de um termo no repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: dbd067dbd3447691fd7fbd8e51670cceb46d64da
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539140"
---
# <a name="localizedlabel-resource-type"></a>tipo de recurso localizedLabel

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o rótulo de um [termo] no [repositório]de termos.

Identifica os rótulos associados a um determinado termo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isDefault|Booliano|Indica se o rótulo é o rótulo padrão.|
|languageTag|Cadeia de Caracteres|A marca anguage do rótulo.|
|nome|String|O nome do rótulo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedLabel",
  "name": "String",
  "isDefault": "Boolean",
  "languageTag": "String"
}
```


[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[microsoft.graph.termStore.store]: termstore-store.md
[terminal]: ../resources/termstore-term.md
[Guarde]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel": "#"
  },
  "suppressions": []
}
-->
