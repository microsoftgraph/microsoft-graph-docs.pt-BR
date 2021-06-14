---
title: Tipo de recurso educationFeedback
description: Comentários de um professor para um aluno.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 471c55668e7849f55d5a7623f86bc1f07fc6e537
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912110"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="3fc08-103">Tipo de recurso educationFeedback</span><span class="sxs-lookup"><span data-stu-id="3fc08-103">educationFeedback resource type</span></span>

<span data-ttu-id="3fc08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fc08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fc08-105">Comentários de um professor para um aluno.</span><span class="sxs-lookup"><span data-stu-id="3fc08-105">Feedback from a teacher to a student.</span></span> 

<span data-ttu-id="3fc08-106">Essa propriedade representa a parte de texto dos comentários juntamente com quem forneceu os comentários.</span><span class="sxs-lookup"><span data-stu-id="3fc08-106">This property represents both the text part of the feedback along with who provided the feedback.</span></span>


## <a name="properties"></a><span data-ttu-id="3fc08-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fc08-107">Properties</span></span>
| <span data-ttu-id="3fc08-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fc08-108">Property</span></span>     | <span data-ttu-id="3fc08-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fc08-109">Type</span></span>   |<span data-ttu-id="3fc08-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fc08-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fc08-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="3fc08-111">feedbackBy</span></span>|[<span data-ttu-id="3fc08-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="3fc08-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="3fc08-113">Usuário que criou os comentários.</span><span class="sxs-lookup"><span data-stu-id="3fc08-113">User who created the feedback.</span></span>|
|<span data-ttu-id="3fc08-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc08-114">feedbackDateTime</span></span>|<span data-ttu-id="3fc08-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc08-115">DateTimeOffset</span></span>|<span data-ttu-id="3fc08-116">Momento no tempo em que os comentários foram dados.</span><span class="sxs-lookup"><span data-stu-id="3fc08-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="3fc08-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3fc08-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3fc08-118">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="3fc08-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="3fc08-119">texto</span><span class="sxs-lookup"><span data-stu-id="3fc08-119">text</span></span>|[<span data-ttu-id="3fc08-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="3fc08-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="3fc08-121">Feedback.</span><span class="sxs-lookup"><span data-stu-id="3fc08-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fc08-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fc08-122">JSON representation</span></span>

<span data-ttu-id="3fc08-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fc08-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String",
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


