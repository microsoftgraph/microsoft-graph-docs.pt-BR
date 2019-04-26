---
title: tipo de recurso educationFeedback
description: Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do comentário junto com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ef923870d94479d7ea1d9d762ee729b5060afd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340494"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="baf55-104">tipo de recurso educationFeedback</span><span class="sxs-lookup"><span data-stu-id="baf55-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baf55-105">Comentários de um professor para um aluno.</span><span class="sxs-lookup"><span data-stu-id="baf55-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="baf55-106">Essa propriedade representa a parte de texto do comentário junto com quem.</span><span class="sxs-lookup"><span data-stu-id="baf55-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="baf55-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="baf55-107">Properties</span></span>
| <span data-ttu-id="baf55-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="baf55-108">Property</span></span>     | <span data-ttu-id="baf55-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="baf55-109">Type</span></span>   |<span data-ttu-id="baf55-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="baf55-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baf55-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="baf55-111">feedbackBy</span></span>|[<span data-ttu-id="baf55-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="baf55-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="baf55-113">Usuário que criou o comentário.</span><span class="sxs-lookup"><span data-stu-id="baf55-113">User who created the feedback.</span></span>|
|<span data-ttu-id="baf55-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="baf55-114">feedbackDateTime</span></span>|<span data-ttu-id="baf55-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baf55-115">DateTimeOffset</span></span>|<span data-ttu-id="baf55-116">Momento no momento em que o comentário foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="baf55-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="baf55-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="baf55-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="baf55-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="baf55-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="baf55-119">texto</span><span class="sxs-lookup"><span data-stu-id="baf55-119">text</span></span>|[<span data-ttu-id="baf55-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="baf55-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="baf55-121">Solicitações.</span><span class="sxs-lookup"><span data-stu-id="baf55-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="baf55-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="baf55-122">JSON representation</span></span>

<span data-ttu-id="baf55-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="baf55-123">The following is a JSON representation of the resource.</span></span>

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
