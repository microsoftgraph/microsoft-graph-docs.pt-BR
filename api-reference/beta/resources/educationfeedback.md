---
title: tipo de recurso de educationFeedback
description: Os comentários feitos durante um professor para um estudante. Essa propriedade representa a parte de texto dos comentários, juntamente com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 96f1e0f4d6be070548d984786042a801d764ece9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962685"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="efb18-104">tipo de recurso de educationFeedback</span><span class="sxs-lookup"><span data-stu-id="efb18-104">educationFeedback resource type</span></span>

> <span data-ttu-id="efb18-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="efb18-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efb18-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="efb18-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efb18-107">Os comentários feitos durante um professor para um estudante.</span><span class="sxs-lookup"><span data-stu-id="efb18-107">Feedback from a teacher to a student.</span></span> <span data-ttu-id="efb18-108">Essa propriedade representa a parte de texto dos comentários, juntamente com quem.</span><span class="sxs-lookup"><span data-stu-id="efb18-108">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="efb18-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efb18-109">Properties</span></span>
| <span data-ttu-id="efb18-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efb18-110">Property</span></span>     | <span data-ttu-id="efb18-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="efb18-111">Type</span></span>   |<span data-ttu-id="efb18-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb18-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efb18-113">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="efb18-113">feedbackBy</span></span>|[<span data-ttu-id="efb18-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="efb18-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="efb18-115">Usuário que criou o feedback.</span><span class="sxs-lookup"><span data-stu-id="efb18-115">User who created the feedback.</span></span>|
|<span data-ttu-id="efb18-116">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="efb18-116">feedbackDateTime</span></span>|<span data-ttu-id="efb18-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efb18-117">DateTimeOffset</span></span>|<span data-ttu-id="efb18-118">Momento específico quando o feedback dado.</span><span class="sxs-lookup"><span data-stu-id="efb18-118">Moment in time when the feedback was given.</span></span> <span data-ttu-id="efb18-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="efb18-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="efb18-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="efb18-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="efb18-121">texto</span><span class="sxs-lookup"><span data-stu-id="efb18-121">text</span></span>|[<span data-ttu-id="efb18-122">itemBody</span><span class="sxs-lookup"><span data-stu-id="efb18-122">itemBody</span></span>](itembody.md)|<span data-ttu-id="efb18-123">Comentários.</span><span class="sxs-lookup"><span data-stu-id="efb18-123">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efb18-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efb18-124">JSON representation</span></span>

<span data-ttu-id="efb18-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efb18-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
