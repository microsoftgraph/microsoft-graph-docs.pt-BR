---
title: tipo de recurso educationAssignmentGrade
description: " no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses dessa"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9680a298c405a81648ba0a5fe95cdf0df0c841bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502743"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="4dc9e-103">tipo de recurso educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="4dc9e-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="4dc9e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4dc9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dc9e-105">Representa o objeto **graduação** em um envio.</span><span class="sxs-lookup"><span data-stu-id="4dc9e-105">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="4dc9e-106">Este é um tipo abstrato que nunca será instanciado; no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses desse tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="4dc9e-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="4dc9e-107">Esse objeto também controla quem está fazendo a gradação.</span><span class="sxs-lookup"><span data-stu-id="4dc9e-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="4dc9e-108">Isso é usado na propriedade **enmisse.**</span><span class="sxs-lookup"><span data-stu-id="4dc9e-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="4dc9e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4dc9e-109">Properties</span></span>
| <span data-ttu-id="4dc9e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dc9e-110">Property</span></span>     | <span data-ttu-id="4dc9e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dc9e-111">Type</span></span>   |<span data-ttu-id="4dc9e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dc9e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dc9e-113">gradedBy</span><span class="sxs-lookup"><span data-stu-id="4dc9e-113">gradedBy</span></span>|[<span data-ttu-id="4dc9e-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="4dc9e-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="4dc9e-115">Usuário que fazia a gradação.</span><span class="sxs-lookup"><span data-stu-id="4dc9e-115">User who did the grading.</span></span> |
|<span data-ttu-id="4dc9e-116">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dc9e-116">gradedDateTime</span></span>|<span data-ttu-id="4dc9e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dc9e-117">DateTimeOffset</span></span>| <span data-ttu-id="4dc9e-118">Momento no momento em que a classificação foi aplicada a este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="4dc9e-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="4dc9e-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4dc9e-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4dc9e-120">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4dc9e-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4dc9e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4dc9e-121">JSON representation</span></span>

<span data-ttu-id="4dc9e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4dc9e-122">The following is a JSON representation of the resource.</span></span>

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
