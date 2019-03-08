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
# <a name="root-resource-type"></a><span data-ttu-id="4422a-102">Tipo de recurso Root</span><span class="sxs-lookup"><span data-stu-id="4422a-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4422a-103">A faceta **Root** indica que um objeto é o mais alto em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="4422a-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="4422a-104">A presença (não nulo) do valor da faceta indica que o objeto é a raiz.</span><span class="sxs-lookup"><span data-stu-id="4422a-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="4422a-105">Um valor nulo (ou ausente) indica que o objeto não é a raiz.</span><span class="sxs-lookup"><span data-stu-id="4422a-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="4422a-106">**Observação**: Embora essa faceta esteja vazia no momento, em revisões futuras da API a faceta pode ser preenchida com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="4422a-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4422a-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4422a-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="4422a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4422a-108">Properties</span></span>

<span data-ttu-id="4422a-109">O recurso **Root** não tem propriedades.</span><span class="sxs-lookup"><span data-stu-id="4422a-109">The **Root** resource has no properties.</span></span>


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
