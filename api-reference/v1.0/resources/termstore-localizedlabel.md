---
title: Tipo de recurso localizedLabel
description: Representa o rótulo de um termo no armazenamento de termos.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: da9e3fb1a3cff98823771c1c99db052b92ba7e38
ms.sourcegitcommit: 998c63e6290cfb5ad4a6bd3eb3e249d282f962a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2021
ms.locfileid: "58533718"
---
# <a name="localizedlabel-resource-type"></a>Tipo de recurso localizedLabel

Namespace: microsoft.graph.termStore

Representa o rótulo de [um termo] no armazenamento de [termos.]

Identifica os rótulos associados a um determinado termo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isDefault|Booliano|Indica se o rótulo é o rótulo padrão.|
|languageTag|Cadeia de caracteres|A marca de idioma do rótulo.|
|nome|Cadeia de caracteres|O nome do rótulo.|

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
[term]: ../resources/termstore-term.md
[store]: ../resources/termstore-store.md


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


