---
title: tipo de recurso educationAssignmentGrade
description: " no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses dessa"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: e925059a5eb06e5cc9795f78368b884fa40dd3ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334526"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="1b07e-103">tipo de recurso educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="1b07e-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b07e-104">Representa o objeto **graduação** em um envio.</span><span class="sxs-lookup"><span data-stu-id="1b07e-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="1b07e-105">Este é um tipo abstrato que nunca será instanciado; no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses desse tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="1b07e-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="1b07e-106">Esse objeto também controla quem está fazendo a gradação.</span><span class="sxs-lookup"><span data-stu-id="1b07e-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="1b07e-107">Isso é usado na propriedade **enmisse.**</span><span class="sxs-lookup"><span data-stu-id="1b07e-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="1b07e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b07e-108">Properties</span></span>
| <span data-ttu-id="1b07e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b07e-109">Property</span></span>     | <span data-ttu-id="1b07e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b07e-110">Type</span></span>   |<span data-ttu-id="1b07e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b07e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b07e-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="1b07e-112">gradedBy</span></span>|[<span data-ttu-id="1b07e-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b07e-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="1b07e-114">Usuário que fazia a gradação.</span><span class="sxs-lookup"><span data-stu-id="1b07e-114">User who did the grading.</span></span> |
|<span data-ttu-id="1b07e-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b07e-115">gradedDateTime</span></span>|<span data-ttu-id="1b07e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b07e-116">DateTimeOffset</span></span>| <span data-ttu-id="1b07e-117">Momento no momento em que a classificação foi aplicada a este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="1b07e-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="1b07e-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1b07e-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1b07e-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1b07e-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b07e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b07e-120">JSON representation</span></span>

<span data-ttu-id="1b07e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b07e-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
