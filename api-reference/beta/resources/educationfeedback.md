---
title: tipo de recurso educationFeedback
description: Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do comentário junto com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: aac921b1e9f70bc22db2b91833a6b6d348a935db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502141"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="3319e-104">tipo de recurso educationFeedback</span><span class="sxs-lookup"><span data-stu-id="3319e-104">educationFeedback resource type</span></span>

<span data-ttu-id="3319e-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3319e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3319e-106">Comentários de um professor para um aluno.</span><span class="sxs-lookup"><span data-stu-id="3319e-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="3319e-107">Essa propriedade representa a parte de texto do comentário junto com quem.</span><span class="sxs-lookup"><span data-stu-id="3319e-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="3319e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3319e-108">Properties</span></span>
| <span data-ttu-id="3319e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3319e-109">Property</span></span>     | <span data-ttu-id="3319e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3319e-110">Type</span></span>   |<span data-ttu-id="3319e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3319e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3319e-112">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="3319e-112">feedbackBy</span></span>|[<span data-ttu-id="3319e-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="3319e-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="3319e-114">Usuário que criou o comentário.</span><span class="sxs-lookup"><span data-stu-id="3319e-114">User who created the feedback.</span></span>|
|<span data-ttu-id="3319e-115">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="3319e-115">feedbackDateTime</span></span>|<span data-ttu-id="3319e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3319e-116">DateTimeOffset</span></span>|<span data-ttu-id="3319e-117">Momento no momento em que o comentário foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="3319e-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="3319e-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3319e-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3319e-119">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3319e-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3319e-120">texto</span><span class="sxs-lookup"><span data-stu-id="3319e-120">text</span></span>|[<span data-ttu-id="3319e-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="3319e-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="3319e-122">Solicitações.</span><span class="sxs-lookup"><span data-stu-id="3319e-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3319e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3319e-123">JSON representation</span></span>

<span data-ttu-id="3319e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3319e-124">The following is a JSON representation of the resource.</span></span>

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
