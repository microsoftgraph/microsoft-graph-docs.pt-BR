---
title: Tipo de recurso educationFeedbackOutcome
description: Um educationOutcome que fornece comentários na forma de texto.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d29a09ccca331e466812c44e8f397696d1eb3539
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912114"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="c1a29-103">Tipo de recurso educationFeedbackOutcome</span><span class="sxs-lookup"><span data-stu-id="c1a29-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="c1a29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1a29-105">Representa comentários em [um objeto educationOutcome](educationoutcome.md) na forma de texto.</span><span class="sxs-lookup"><span data-stu-id="c1a29-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="c1a29-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c1a29-106">Methods</span></span>

| <span data-ttu-id="c1a29-107">Método</span><span class="sxs-lookup"><span data-stu-id="c1a29-107">Method</span></span>       | <span data-ttu-id="c1a29-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c1a29-108">Return Type</span></span> | <span data-ttu-id="c1a29-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a29-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c1a29-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="c1a29-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="c1a29-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="c1a29-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="c1a29-112">Atualizar o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="c1a29-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c1a29-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1a29-113">Properties</span></span>

| <span data-ttu-id="c1a29-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1a29-114">Property</span></span>     | <span data-ttu-id="c1a29-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1a29-115">Type</span></span>        | <span data-ttu-id="c1a29-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a29-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1a29-117">comentários</span><span class="sxs-lookup"><span data-stu-id="c1a29-117">feedback</span></span>|[<span data-ttu-id="c1a29-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="c1a29-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="c1a29-119">Comentários escritos do professor para o aluno.</span><span class="sxs-lookup"><span data-stu-id="c1a29-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="c1a29-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="c1a29-120">publishedFeedback</span></span>|[<span data-ttu-id="c1a29-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="c1a29-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="c1a29-122">Uma cópia da propriedade feedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="c1a29-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1a29-123">Relações</span><span class="sxs-lookup"><span data-stu-id="c1a29-123">Relationships</span></span>

<span data-ttu-id="c1a29-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1a29-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1a29-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1a29-125">JSON representation</span></span>

<span data-ttu-id="c1a29-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1a29-126">The following is a JSON representation of the resource.</span></span>

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

