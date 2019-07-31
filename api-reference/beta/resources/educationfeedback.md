---
title: tipo de recurso educationFeedback
description: Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do comentário junto com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7300c5f2d46a3a60a104288d8ee9559e6cf5fd2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006413"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="53857-104">tipo de recurso educationFeedback</span><span class="sxs-lookup"><span data-stu-id="53857-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53857-105">Comentários de um professor para um aluno.</span><span class="sxs-lookup"><span data-stu-id="53857-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="53857-106">Essa propriedade representa a parte de texto do comentário junto com quem.</span><span class="sxs-lookup"><span data-stu-id="53857-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="53857-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53857-107">Properties</span></span>
| <span data-ttu-id="53857-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53857-108">Property</span></span>     | <span data-ttu-id="53857-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="53857-109">Type</span></span>   |<span data-ttu-id="53857-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="53857-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53857-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="53857-111">feedbackBy</span></span>|[<span data-ttu-id="53857-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="53857-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="53857-113">Usuário que criou o comentário.</span><span class="sxs-lookup"><span data-stu-id="53857-113">User who created the feedback.</span></span>|
|<span data-ttu-id="53857-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="53857-114">feedbackDateTime</span></span>|<span data-ttu-id="53857-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53857-115">DateTimeOffset</span></span>|<span data-ttu-id="53857-116">Momento no momento em que o comentário foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="53857-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="53857-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="53857-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53857-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="53857-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="53857-119">texto</span><span class="sxs-lookup"><span data-stu-id="53857-119">text</span></span>|[<span data-ttu-id="53857-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="53857-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="53857-121">Solicitações.</span><span class="sxs-lookup"><span data-stu-id="53857-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53857-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53857-122">JSON representation</span></span>

<span data-ttu-id="53857-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53857-123">The following is a JSON representation of the resource.</span></span>

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
