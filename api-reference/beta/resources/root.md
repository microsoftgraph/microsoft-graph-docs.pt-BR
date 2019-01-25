---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Raiz
localization_priority: Normal
ms.openlocfilehash: dda2de3e92128a9813f923d9acfef0eec94680e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510299"
---
# <a name="root-resource-type"></a><span data-ttu-id="45b1d-102">Tipo de recurso Root</span><span class="sxs-lookup"><span data-stu-id="45b1d-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45b1d-103">A faceta **Root** indica que um objeto é o mais alto em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="45b1d-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="45b1d-104">A presença (não nulo) do valor da faceta indica que o objeto é a raiz.</span><span class="sxs-lookup"><span data-stu-id="45b1d-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="45b1d-105">Um valor nulo (ou ausente) indica que o objeto não é a raiz.</span><span class="sxs-lookup"><span data-stu-id="45b1d-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="45b1d-106">**Observação**: Embora essa faceta esteja vazia no momento, em revisões futuras da API a faceta pode ser preenchida com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="45b1d-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="45b1d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45b1d-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="45b1d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45b1d-108">Properties</span></span>

<span data-ttu-id="45b1d-109">O recurso **Root** não tem propriedades.</span><span class="sxs-lookup"><span data-stu-id="45b1d-109">The **Root** resource has no properties.</span></span>


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
