---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 683a290806f9a70f97bda4aa9429a64578fbcd97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463555"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="68291-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="68291-103">educationStudent resource type</span></span>

<span data-ttu-id="68291-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="68291-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="68291-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68291-105">Properties</span></span>
| <span data-ttu-id="68291-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68291-106">Property</span></span>     | <span data-ttu-id="68291-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="68291-107">Type</span></span>   |<span data-ttu-id="68291-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="68291-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68291-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="68291-109">birthDate</span></span>|<span data-ttu-id="68291-110">Data</span><span class="sxs-lookup"><span data-stu-id="68291-110">Date</span></span>| <span data-ttu-id="68291-111">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="68291-111">Birth date of the student.</span></span>|
|<span data-ttu-id="68291-112">externalId</span><span class="sxs-lookup"><span data-stu-id="68291-112">externalId</span></span>|<span data-ttu-id="68291-113">String</span><span class="sxs-lookup"><span data-stu-id="68291-113">String</span></span>| <span data-ttu-id="68291-114">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="68291-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="68291-115">gender</span><span class="sxs-lookup"><span data-stu-id="68291-115">gender</span></span>|<span data-ttu-id="68291-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="68291-116">educationGender</span></span>| <span data-ttu-id="68291-117">Os valores possíveis são: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="68291-117">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="68291-118">grade</span><span class="sxs-lookup"><span data-stu-id="68291-118">grade</span></span>|<span data-ttu-id="68291-119">String</span><span class="sxs-lookup"><span data-stu-id="68291-119">String</span></span>|<span data-ttu-id="68291-120">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="68291-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="68291-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="68291-121">graduationYear</span></span>|<span data-ttu-id="68291-122">String</span><span class="sxs-lookup"><span data-stu-id="68291-122">String</span></span>| <span data-ttu-id="68291-123">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="68291-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="68291-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="68291-124">studentNumber</span></span>|<span data-ttu-id="68291-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68291-125">String</span></span>| <span data-ttu-id="68291-126">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="68291-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68291-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68291-127">JSON representation</span></span>

<span data-ttu-id="68291-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68291-128">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
