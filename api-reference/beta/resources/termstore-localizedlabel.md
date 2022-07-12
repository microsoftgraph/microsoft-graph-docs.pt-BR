---
title: Tipo de recurso localizedLabel
description: Representa o rótulo de um termo no repositório de termos.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 1317d51a113da35289b06b035c43316059edf7d0
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731558"
---
# <a name="localizedlabel-resource-type"></a>Tipo de recurso localizedLabel

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o rótulo de um [termo] no repositório de [termos].

Identifica os rótulos associados a um determinado termo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isDefault|Booliano|Indica se o rótulo é o rótulo padrão.|
|languageTag|String|A marca de idioma do rótulo.|
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
[Termo]: ../resources/termstore-term.md
[Loja]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel&quot;: &quot;#"
  },
  "suppressions": []
}
-->


