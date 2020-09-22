---
title: tipo de recurso educationOutcome
description: O resultado da gradação de uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 129e48b5d1101aaf9ab6ab7eb8c89a92b41a6ac7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081707"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="6ea34-103">tipo de recurso educationOutcome</span><span class="sxs-lookup"><span data-stu-id="6ea34-103">educationOutcome resource type</span></span>

<span data-ttu-id="6ea34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ea34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ea34-105">O resultado da gradação de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="6ea34-105">The result of grading an assignment.</span></span> <span data-ttu-id="6ea34-106">Esta é uma classe base; os tipos derivados são [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md)e [educationRubricOutcome](educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="6ea34-106">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6ea34-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6ea34-107">Methods</span></span>

| <span data-ttu-id="6ea34-108">Método</span><span class="sxs-lookup"><span data-stu-id="6ea34-108">Method</span></span>       | <span data-ttu-id="6ea34-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6ea34-109">Return Type</span></span> | <span data-ttu-id="6ea34-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea34-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6ea34-111">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="6ea34-111">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="6ea34-112">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="6ea34-112">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="6ea34-113">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="6ea34-113">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6ea34-114">Relações</span><span class="sxs-lookup"><span data-stu-id="6ea34-114">Relationships</span></span>

<span data-ttu-id="6ea34-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ea34-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ea34-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ea34-116">JSON representation</span></span>

<span data-ttu-id="6ea34-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ea34-117">The following is a JSON representation of the resource.</span></span>

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

