---
title: tipo de recurso educationFeedbackOutcome
description: Um educationOutcome que fornece comentários na forma de texto.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b1b768fbb87804d2df16e6300cc14d71283461c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095461"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="4e519-103">tipo de recurso educationFeedbackOutcome</span><span class="sxs-lookup"><span data-stu-id="4e519-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="4e519-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e519-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e519-105">Representa comentários sobre um objeto [educationOutcome](educationoutcome.md) na forma de texto.</span><span class="sxs-lookup"><span data-stu-id="4e519-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="4e519-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="4e519-106">Methods</span></span>

| <span data-ttu-id="4e519-107">Método</span><span class="sxs-lookup"><span data-stu-id="4e519-107">Method</span></span>       | <span data-ttu-id="4e519-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4e519-108">Return Type</span></span> | <span data-ttu-id="4e519-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e519-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4e519-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="4e519-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="4e519-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="4e519-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="4e519-112">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="4e519-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e519-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e519-113">Properties</span></span>

| <span data-ttu-id="4e519-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e519-114">Property</span></span>     | <span data-ttu-id="4e519-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e519-115">Type</span></span>        | <span data-ttu-id="4e519-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e519-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4e519-117">comentários</span><span class="sxs-lookup"><span data-stu-id="4e519-117">feedback</span></span>|[<span data-ttu-id="4e519-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="4e519-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="4e519-119">Comentários escritos do professor para o aluno.</span><span class="sxs-lookup"><span data-stu-id="4e519-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="4e519-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="4e519-120">publishedFeedback</span></span>|[<span data-ttu-id="4e519-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="4e519-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="4e519-122">Uma cópia da propriedade feedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="4e519-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e519-123">Relações</span><span class="sxs-lookup"><span data-stu-id="4e519-123">Relationships</span></span>

<span data-ttu-id="4e519-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e519-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e519-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e519-125">JSON representation</span></span>

<span data-ttu-id="4e519-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e519-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "baseType": "",
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

