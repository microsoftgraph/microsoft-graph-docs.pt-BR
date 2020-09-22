---
title: tipo de recurso educationFeedback
description: Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do comentário junto com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00514ce99860fa52d167465fb223dad2981c28db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095475"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="bdd36-104">tipo de recurso educationFeedback</span><span class="sxs-lookup"><span data-stu-id="bdd36-104">educationFeedback resource type</span></span>

<span data-ttu-id="bdd36-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdd36-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd36-106">Comentários de um professor para um aluno.</span><span class="sxs-lookup"><span data-stu-id="bdd36-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="bdd36-107">Essa propriedade representa a parte de texto do comentário junto com quem.</span><span class="sxs-lookup"><span data-stu-id="bdd36-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="bdd36-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdd36-108">Properties</span></span>
| <span data-ttu-id="bdd36-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdd36-109">Property</span></span>     | <span data-ttu-id="bdd36-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdd36-110">Type</span></span>   |<span data-ttu-id="bdd36-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd36-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdd36-112">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="bdd36-112">feedbackBy</span></span>|[<span data-ttu-id="bdd36-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="bdd36-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="bdd36-114">Usuário que criou o comentário.</span><span class="sxs-lookup"><span data-stu-id="bdd36-114">User who created the feedback.</span></span>|
|<span data-ttu-id="bdd36-115">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="bdd36-115">feedbackDateTime</span></span>|<span data-ttu-id="bdd36-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdd36-116">DateTimeOffset</span></span>|<span data-ttu-id="bdd36-117">Momento no momento em que o comentário foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="bdd36-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="bdd36-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bdd36-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bdd36-119">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bdd36-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bdd36-120">texto</span><span class="sxs-lookup"><span data-stu-id="bdd36-120">text</span></span>|[<span data-ttu-id="bdd36-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="bdd36-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="bdd36-122">Solicitações.</span><span class="sxs-lookup"><span data-stu-id="bdd36-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdd36-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdd36-123">JSON representation</span></span>

<span data-ttu-id="bdd36-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdd36-124">The following is a JSON representation of the resource.</span></span>

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


