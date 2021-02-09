---
title: Tipo de recurso educationFeedbackOutcome
description: Um educationOutcome que fornece comentários na forma de texto.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c50776f6b8dde27d8f937e8b7ee2028ce1cfca1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153639"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="e61d5-103">Tipo de recurso educationFeedbackOutcome</span><span class="sxs-lookup"><span data-stu-id="e61d5-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="e61d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e61d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e61d5-105">Representa comentários sobre [um objeto educationOutcome](educationoutcome.md) na forma de texto.</span><span class="sxs-lookup"><span data-stu-id="e61d5-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="e61d5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e61d5-106">Methods</span></span>

| <span data-ttu-id="e61d5-107">Método</span><span class="sxs-lookup"><span data-stu-id="e61d5-107">Method</span></span>       | <span data-ttu-id="e61d5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e61d5-108">Return Type</span></span> | <span data-ttu-id="e61d5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e61d5-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e61d5-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="e61d5-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="e61d5-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="e61d5-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="e61d5-112">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="e61d5-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e61d5-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e61d5-113">Properties</span></span>

| <span data-ttu-id="e61d5-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e61d5-114">Property</span></span>     | <span data-ttu-id="e61d5-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e61d5-115">Type</span></span>        | <span data-ttu-id="e61d5-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e61d5-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e61d5-117">comentários</span><span class="sxs-lookup"><span data-stu-id="e61d5-117">feedback</span></span>|[<span data-ttu-id="e61d5-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="e61d5-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="e61d5-119">Comentários escritos pelo professor para o aluno.</span><span class="sxs-lookup"><span data-stu-id="e61d5-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="e61d5-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="e61d5-120">publishedFeedback</span></span>|[<span data-ttu-id="e61d5-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="e61d5-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="e61d5-122">Uma cópia da propriedade de feedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="e61d5-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e61d5-123">Relações</span><span class="sxs-lookup"><span data-stu-id="e61d5-123">Relationships</span></span>

<span data-ttu-id="e61d5-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e61d5-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e61d5-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e61d5-125">JSON representation</span></span>

<span data-ttu-id="e61d5-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e61d5-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

