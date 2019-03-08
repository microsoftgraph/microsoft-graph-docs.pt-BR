---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Jailbreak
localization_priority: Normal
ms.openlocfilehash: 8c320a34d22af5fc73a1c5d8c96dce14e176946f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482368"
---
# <a name="root-resource-type"></a>Tipo de recurso Root

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A faceta **Root** indica que um objeto é o mais alto em sua hierarquia.
A presença (não nulo) do valor da faceta indica que o objeto é a raiz.
Um valor nulo (ou ausente) indica que o objeto não é a raiz.

**Observação**: Embora essa faceta esteja vazia no momento, em revisões futuras da API a faceta pode ser preenchida com propriedades adicionais.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a>Propriedades

O recurso **Root** não tem propriedades.


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": [
    "Error: /api-reference/beta/resources/root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
