---
title: tipo de recurso educationAssignmentGrade
description: " no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses dessa"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5ca13ba057ef000a468d910d49288d9ae8e0c962
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543018"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="acca9-103">tipo de recurso educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="acca9-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acca9-104">Representa o objeto **graduação** em um envio.</span><span class="sxs-lookup"><span data-stu-id="acca9-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="acca9-105">Este é um tipo abstrato que nunca será instanciado; no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses desse tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="acca9-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="acca9-106">Esse objeto também controla quem está fazendo a gradação.</span><span class="sxs-lookup"><span data-stu-id="acca9-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="acca9-107">Isso é usado na propriedade **enmisse.**</span><span class="sxs-lookup"><span data-stu-id="acca9-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="acca9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acca9-108">Properties</span></span>
| <span data-ttu-id="acca9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acca9-109">Property</span></span>     | <span data-ttu-id="acca9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="acca9-110">Type</span></span>   |<span data-ttu-id="acca9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="acca9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acca9-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="acca9-112">gradedBy</span></span>|[<span data-ttu-id="acca9-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="acca9-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="acca9-114">Usuário que fazia a gradação.</span><span class="sxs-lookup"><span data-stu-id="acca9-114">User who did the grading.</span></span> |
|<span data-ttu-id="acca9-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="acca9-115">gradedDateTime</span></span>|<span data-ttu-id="acca9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acca9-116">DateTimeOffset</span></span>| <span data-ttu-id="acca9-117">Momento no momento em que a classificação foi aplicada a este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="acca9-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="acca9-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="acca9-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="acca9-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="acca9-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acca9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acca9-120">JSON representation</span></span>

<span data-ttu-id="acca9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acca9-121">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
