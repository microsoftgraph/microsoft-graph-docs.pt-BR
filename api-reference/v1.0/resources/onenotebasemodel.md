---
title: recurso de onenoteEntityBaseModel
description: Este é o tipo de base para entidades do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 53ed86ae22f3ac9fccdef98e56382cd9440e71e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923128"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="a2133-103">recurso de onenoteEntityBaseModel</span><span class="sxs-lookup"><span data-stu-id="a2133-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="a2133-104">Este é o tipo de base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="a2133-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2133-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2133-105">JSON representation</span></span>

<span data-ttu-id="a2133-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2133-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="a2133-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2133-107">Properties</span></span>
| <span data-ttu-id="a2133-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2133-108">Property</span></span>     | <span data-ttu-id="a2133-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2133-109">Type</span></span>   |<span data-ttu-id="a2133-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2133-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2133-111">self</span><span class="sxs-lookup"><span data-stu-id="a2133-111">self</span></span>|<span data-ttu-id="a2133-112">String</span><span class="sxs-lookup"><span data-stu-id="a2133-112">String</span></span>|<span data-ttu-id="a2133-p101">O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2133-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
