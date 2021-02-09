---
title: Tipo de recurso educationOutcome
description: O resultado da gradação de uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 788985e5e63272fea31e579c2da4472ec065dfc5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153618"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="18815-103">Tipo de recurso educationOutcome</span><span class="sxs-lookup"><span data-stu-id="18815-103">educationOutcome resource type</span></span>

<span data-ttu-id="18815-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18815-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18815-105">O resultado da gradação de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="18815-105">The result of grading an assignment.</span></span> <span data-ttu-id="18815-106">Esta é uma classe base; os tipos derivados [são educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md)e [educationRubricOutcome](educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="18815-106">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="18815-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="18815-107">Methods</span></span>

| <span data-ttu-id="18815-108">Método</span><span class="sxs-lookup"><span data-stu-id="18815-108">Method</span></span>       | <span data-ttu-id="18815-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18815-109">Return Type</span></span> | <span data-ttu-id="18815-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18815-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="18815-111">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="18815-111">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="18815-112">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="18815-112">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="18815-113">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="18815-113">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="18815-114">Relações</span><span class="sxs-lookup"><span data-stu-id="18815-114">Relationships</span></span>

<span data-ttu-id="18815-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18815-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18815-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18815-116">JSON representation</span></span>

<span data-ttu-id="18815-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18815-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
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

