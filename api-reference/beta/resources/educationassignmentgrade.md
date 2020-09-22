---
title: tipo de recurso educationAssignmentGrade
description: " no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses dessa"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41e981d268718a94e6b28df6b43c4c2f931b7ad2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013745"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="a49df-103">tipo de recurso educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="a49df-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="a49df-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a49df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a49df-105">Representa o objeto **graduação** em um envio.</span><span class="sxs-lookup"><span data-stu-id="a49df-105">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="a49df-106">Este é um tipo abstrato que nunca será instanciado; no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses desse tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="a49df-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="a49df-107">Esse objeto também controla quem está fazendo a gradação.</span><span class="sxs-lookup"><span data-stu-id="a49df-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="a49df-108">Isso é usado na propriedade **enmisse.**</span><span class="sxs-lookup"><span data-stu-id="a49df-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="a49df-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a49df-109">Properties</span></span>
| <span data-ttu-id="a49df-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a49df-110">Property</span></span>     | <span data-ttu-id="a49df-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a49df-111">Type</span></span>   |<span data-ttu-id="a49df-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a49df-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a49df-113">gradedBy</span><span class="sxs-lookup"><span data-stu-id="a49df-113">gradedBy</span></span>|[<span data-ttu-id="a49df-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="a49df-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="a49df-115">Usuário que fazia a gradação.</span><span class="sxs-lookup"><span data-stu-id="a49df-115">User who did the grading.</span></span> |
|<span data-ttu-id="a49df-116">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="a49df-116">gradedDateTime</span></span>|<span data-ttu-id="a49df-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49df-117">DateTimeOffset</span></span>| <span data-ttu-id="a49df-118">Momento no momento em que a classificação foi aplicada a este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="a49df-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="a49df-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a49df-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a49df-120">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a49df-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a49df-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a49df-121">JSON representation</span></span>

<span data-ttu-id="a49df-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a49df-122">The following is a JSON representation of the resource.</span></span>

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


