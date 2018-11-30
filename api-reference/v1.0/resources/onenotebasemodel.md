---
title: recurso de onenoteEntityBaseModel
description: Este é o tipo de base para entidades do OneNote.
ms.openlocfilehash: 68a864437cec59d9b5f0d3e69161b49bca80231c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004968"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="a25c1-103">recurso de onenoteEntityBaseModel</span><span class="sxs-lookup"><span data-stu-id="a25c1-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="a25c1-104">Este é o tipo de base para entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="a25c1-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a25c1-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a25c1-105">JSON representation</span></span>

<span data-ttu-id="a25c1-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a25c1-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a25c1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a25c1-107">Properties</span></span>
| <span data-ttu-id="a25c1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a25c1-108">Property</span></span>     | <span data-ttu-id="a25c1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a25c1-109">Type</span></span>   |<span data-ttu-id="a25c1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a25c1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a25c1-111">self</span><span class="sxs-lookup"><span data-stu-id="a25c1-111">self</span></span>|<span data-ttu-id="a25c1-112">String</span><span class="sxs-lookup"><span data-stu-id="a25c1-112">String</span></span>|<span data-ttu-id="a25c1-p101">O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a25c1-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->