---
title: tipo de recurso educationFeedback
description: Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do comentário junto com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 90e55b20b371d04bc3c6d45bb84fe6bf42157a2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507135"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="9a361-104">tipo de recurso educationFeedback</span><span class="sxs-lookup"><span data-stu-id="9a361-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a361-105">Comentários de um professor para um aluno.</span><span class="sxs-lookup"><span data-stu-id="9a361-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="9a361-106">Essa propriedade representa a parte de texto do comentário junto com quem.</span><span class="sxs-lookup"><span data-stu-id="9a361-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="9a361-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a361-107">Properties</span></span>
| <span data-ttu-id="9a361-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a361-108">Property</span></span>     | <span data-ttu-id="9a361-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a361-109">Type</span></span>   |<span data-ttu-id="9a361-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a361-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a361-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="9a361-111">feedbackBy</span></span>|[<span data-ttu-id="9a361-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a361-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="9a361-113">Usuário que criou o comentário.</span><span class="sxs-lookup"><span data-stu-id="9a361-113">User who created the feedback.</span></span>|
|<span data-ttu-id="9a361-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="9a361-114">feedbackDateTime</span></span>|<span data-ttu-id="9a361-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a361-115">DateTimeOffset</span></span>|<span data-ttu-id="9a361-116">Momento no momento em que o comentário foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="9a361-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="9a361-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9a361-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a361-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a361-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a361-119">texto</span><span class="sxs-lookup"><span data-stu-id="9a361-119">text</span></span>|[<span data-ttu-id="9a361-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="9a361-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="9a361-121">Solicitações.</span><span class="sxs-lookup"><span data-stu-id="9a361-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a361-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a361-122">JSON representation</span></span>

<span data-ttu-id="9a361-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a361-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfeedback.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
