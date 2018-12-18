---
title: recurso de onenoteEntityBaseModel
description: Este é o tipo de base para entidades do OneNote.
author: Jewan-microsoft
ms.openlocfilehash: 25e2da6732fd831c6bbec5ae86bddeae7b702aa5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310462"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="0058d-103">recurso de onenoteEntityBaseModel</span><span class="sxs-lookup"><span data-stu-id="0058d-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="0058d-104">Este é o tipo de base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="0058d-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0058d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0058d-105">JSON representation</span></span>

<span data-ttu-id="0058d-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0058d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0058d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0058d-107">Properties</span></span>
| <span data-ttu-id="0058d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0058d-108">Property</span></span>     | <span data-ttu-id="0058d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0058d-109">Type</span></span>   |<span data-ttu-id="0058d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0058d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0058d-111">self</span><span class="sxs-lookup"><span data-stu-id="0058d-111">self</span></span>|<span data-ttu-id="0058d-112">String</span><span class="sxs-lookup"><span data-stu-id="0058d-112">String</span></span>|<span data-ttu-id="0058d-p101">O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0058d-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->