---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 554763d41c4ce48a09334394330e05fcd6dd4152
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507116"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="396eb-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="396eb-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="396eb-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="396eb-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="396eb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="396eb-105">Properties</span></span>
| <span data-ttu-id="396eb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="396eb-106">Property</span></span>     | <span data-ttu-id="396eb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="396eb-107">Type</span></span>   |<span data-ttu-id="396eb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="396eb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="396eb-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="396eb-109">birthDate</span></span>|<span data-ttu-id="396eb-110">Data</span><span class="sxs-lookup"><span data-stu-id="396eb-110">Date</span></span>| <span data-ttu-id="396eb-111">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="396eb-111">Birth date of the student.</span></span>|
|<span data-ttu-id="396eb-112">externalId</span><span class="sxs-lookup"><span data-stu-id="396eb-112">externalId</span></span>|<span data-ttu-id="396eb-113">String</span><span class="sxs-lookup"><span data-stu-id="396eb-113">String</span></span>| <span data-ttu-id="396eb-114">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="396eb-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="396eb-115">gender</span><span class="sxs-lookup"><span data-stu-id="396eb-115">gender</span></span>|<span data-ttu-id="396eb-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="396eb-116">educationGender</span></span>| <span data-ttu-id="396eb-117">Os valores possíveis são: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="396eb-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="396eb-118">grade</span><span class="sxs-lookup"><span data-stu-id="396eb-118">grade</span></span>|<span data-ttu-id="396eb-119">String</span><span class="sxs-lookup"><span data-stu-id="396eb-119">String</span></span>|<span data-ttu-id="396eb-120">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="396eb-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="396eb-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="396eb-121">graduationYear</span></span>|<span data-ttu-id="396eb-122">String</span><span class="sxs-lookup"><span data-stu-id="396eb-122">String</span></span>| <span data-ttu-id="396eb-123">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="396eb-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="396eb-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="396eb-124">studentNumber</span></span>|<span data-ttu-id="396eb-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="396eb-125">String</span></span>| <span data-ttu-id="396eb-126">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="396eb-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="396eb-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="396eb-127">JSON representation</span></span>

<span data-ttu-id="396eb-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="396eb-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationstudent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
