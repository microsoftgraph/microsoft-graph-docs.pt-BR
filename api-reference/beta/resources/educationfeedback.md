---
title: Tipo de recurso educationFeedback
description: Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do feedback juntamente com o quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3ee5e30ddccc215fda7e08cfa4c8c9e7835f1139
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720904"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="8ba6d-104">Tipo de recurso educationFeedback</span><span class="sxs-lookup"><span data-stu-id="8ba6d-104">educationFeedback resource type</span></span>

<span data-ttu-id="8ba6d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ba6d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ba6d-106">Comentários de um professor para um aluno.</span><span class="sxs-lookup"><span data-stu-id="8ba6d-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="8ba6d-107">Essa propriedade representa a parte de texto do feedback juntamente com o quem.</span><span class="sxs-lookup"><span data-stu-id="8ba6d-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="8ba6d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ba6d-108">Properties</span></span>
| <span data-ttu-id="8ba6d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ba6d-109">Property</span></span>     | <span data-ttu-id="8ba6d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ba6d-110">Type</span></span>   |<span data-ttu-id="8ba6d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ba6d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ba6d-112">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="8ba6d-112">feedbackBy</span></span>|[<span data-ttu-id="8ba6d-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="8ba6d-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="8ba6d-114">Usuário que criou os comentários.</span><span class="sxs-lookup"><span data-stu-id="8ba6d-114">User who created the feedback.</span></span>|
|<span data-ttu-id="8ba6d-115">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="8ba6d-115">feedbackDateTime</span></span>|<span data-ttu-id="8ba6d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ba6d-116">DateTimeOffset</span></span>|<span data-ttu-id="8ba6d-117">Momento no tempo em que os comentários foram dados.</span><span class="sxs-lookup"><span data-stu-id="8ba6d-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="8ba6d-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8ba6d-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8ba6d-119">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="8ba6d-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8ba6d-120">texto</span><span class="sxs-lookup"><span data-stu-id="8ba6d-120">text</span></span>|[<span data-ttu-id="8ba6d-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="8ba6d-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="8ba6d-122">Comentários.</span><span class="sxs-lookup"><span data-stu-id="8ba6d-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ba6d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ba6d-123">JSON representation</span></span>

<span data-ttu-id="8ba6d-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ba6d-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String (timestamp)",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


