---
title: tipo de recurso educationAssignmentGrade
description: " no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses dessa"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4de74fc9cbdf505bd57cfad3ab8dbf5a12e4e58a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006469"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="83106-103">tipo de recurso educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="83106-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83106-104">Representa o objeto **graduação** em um envio.</span><span class="sxs-lookup"><span data-stu-id="83106-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="83106-105">Este é um tipo abstrato que nunca será instanciado; no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses desse tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="83106-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="83106-106">Esse objeto também controla quem está fazendo a gradação.</span><span class="sxs-lookup"><span data-stu-id="83106-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="83106-107">Isso é usado na propriedade **enmisse.**</span><span class="sxs-lookup"><span data-stu-id="83106-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="83106-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83106-108">Properties</span></span>
| <span data-ttu-id="83106-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83106-109">Property</span></span>     | <span data-ttu-id="83106-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="83106-110">Type</span></span>   |<span data-ttu-id="83106-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83106-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83106-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="83106-112">gradedBy</span></span>|[<span data-ttu-id="83106-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="83106-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="83106-114">Usuário que fazia a gradação.</span><span class="sxs-lookup"><span data-stu-id="83106-114">User who did the grading.</span></span> |
|<span data-ttu-id="83106-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="83106-115">gradedDateTime</span></span>|<span data-ttu-id="83106-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83106-116">DateTimeOffset</span></span>| <span data-ttu-id="83106-117">Momento no momento em que a classificação foi aplicada a este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="83106-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="83106-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="83106-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="83106-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="83106-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83106-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83106-120">JSON representation</span></span>

<span data-ttu-id="83106-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83106-121">The following is a JSON representation of the resource.</span></span>

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
