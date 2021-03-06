---
title: Tipo de recurso translationLanguageOverride
description: Um recurso que representa uma entrada na lista de substituição de idioma de conversão.
localization_priority: Normal
author: jasonbro
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 791908546c64cbb0ea7ee7434bece3dca5c894cc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518138"
---
# <a name="translationlanguageoverride-resource-type"></a>Tipo de recurso translationLanguageOverride

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa qualquer substituição de conversão para um idioma.

## <a name="properties"></a>Propriedades

|Propriedade             |Tipo                                         |Descrição                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|languageTag          |Cadeia de caracteres                                       |O idioma para aplicar a substituição.<br><br>Retornado por padrão. Não anulável.       |                   
|translationBehavior  |[translationBehavior](translationPreferences.md#translationbehavior-values)        |O comportamento de substituição de conversão para o idioma, se for o caso.<br><br>Retornado por padrão. Não anulável.|

## <a name="json-representation"></a>Representação JSON

A seguir está uma definição JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationLanguageOverride"
}-->

```json
{
    "languageTag": "string",
    "translationBehavior": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationLanguageOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


