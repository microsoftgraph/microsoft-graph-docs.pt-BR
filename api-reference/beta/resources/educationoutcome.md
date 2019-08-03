---
title: tipo de recurso educationOutcome
description: O resultado da gradação de uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a0a49b9a383f1e787fd2698c6d2011e11b3abedb
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173360"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="dbb55-103">tipo de recurso educationOutcome</span><span class="sxs-lookup"><span data-stu-id="dbb55-103">educationOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbb55-104">O resultado da gradação de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="dbb55-104">The result of grading an assignment.</span></span> <span data-ttu-id="dbb55-105">Esta é uma classe base; os tipos derivados são [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md)e [educationRubricOutcome](educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="dbb55-105">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dbb55-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dbb55-106">Methods</span></span>

| <span data-ttu-id="dbb55-107">Método</span><span class="sxs-lookup"><span data-stu-id="dbb55-107">Method</span></span>       | <span data-ttu-id="dbb55-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dbb55-108">Return Type</span></span> | <span data-ttu-id="dbb55-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb55-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dbb55-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="dbb55-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="dbb55-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="dbb55-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="dbb55-112">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="dbb55-112">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dbb55-113">Relações</span><span class="sxs-lookup"><span data-stu-id="dbb55-113">Relationships</span></span>

<span data-ttu-id="dbb55-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dbb55-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbb55-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbb55-115">JSON representation</span></span>

<span data-ttu-id="dbb55-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbb55-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->