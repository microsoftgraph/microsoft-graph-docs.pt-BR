---
title: tipo de recurso educationFeedbackOutcome
description: Um educationOutcome que fornece comentários na forma de texto.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e61538a62a1bb267b0a13b98b17e9b69a8ceed92
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173248"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="7a33d-103">tipo de recurso educationFeedbackOutcome</span><span class="sxs-lookup"><span data-stu-id="7a33d-103">educationFeedbackOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a33d-104">Representa comentários sobre um objeto [educationOutcome](educationoutcome.md) na forma de texto.</span><span class="sxs-lookup"><span data-stu-id="7a33d-104">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="7a33d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7a33d-105">Methods</span></span>

| <span data-ttu-id="7a33d-106">Método</span><span class="sxs-lookup"><span data-stu-id="7a33d-106">Method</span></span>       | <span data-ttu-id="7a33d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7a33d-107">Return Type</span></span> | <span data-ttu-id="7a33d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a33d-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7a33d-109">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="7a33d-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="7a33d-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="7a33d-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="7a33d-111">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="7a33d-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7a33d-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a33d-112">Properties</span></span>

| <span data-ttu-id="7a33d-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a33d-113">Property</span></span>     | <span data-ttu-id="7a33d-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a33d-114">Type</span></span>        | <span data-ttu-id="7a33d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a33d-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a33d-116">comentários</span><span class="sxs-lookup"><span data-stu-id="7a33d-116">feedback</span></span>|[<span data-ttu-id="7a33d-117">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="7a33d-117">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="7a33d-118">Comentários escritos do professor para o aluno.</span><span class="sxs-lookup"><span data-stu-id="7a33d-118">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="7a33d-119">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="7a33d-119">publishedFeedback</span></span>|[<span data-ttu-id="7a33d-120">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="7a33d-120">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="7a33d-121">Uma cópia da propriedade feedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="7a33d-121">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a33d-122">Relações</span><span class="sxs-lookup"><span data-stu-id="7a33d-122">Relationships</span></span>

<span data-ttu-id="7a33d-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a33d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a33d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a33d-124">JSON representation</span></span>

<span data-ttu-id="7a33d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a33d-125">The following is a JSON representation of the resource.</span></span>

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