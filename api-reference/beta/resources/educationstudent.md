---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dda08acb0a390bfb8b26d88de15aac72dfa1f5f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972534"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="ed7e9-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="ed7e9-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed7e9-104">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="ed7e9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed7e9-105">Properties</span></span>
| <span data-ttu-id="ed7e9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed7e9-106">Property</span></span>     | <span data-ttu-id="ed7e9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed7e9-107">Type</span></span>   |<span data-ttu-id="ed7e9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed7e9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed7e9-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="ed7e9-109">birthDate</span></span>|<span data-ttu-id="ed7e9-110">Data</span><span class="sxs-lookup"><span data-stu-id="ed7e9-110">Date</span></span>| <span data-ttu-id="ed7e9-111">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-111">Birth date of the student.</span></span>|
|<span data-ttu-id="ed7e9-112">externalId</span><span class="sxs-lookup"><span data-stu-id="ed7e9-112">externalId</span></span>|<span data-ttu-id="ed7e9-113">String</span><span class="sxs-lookup"><span data-stu-id="ed7e9-113">String</span></span>| <span data-ttu-id="ed7e9-114">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="ed7e9-115">gender</span><span class="sxs-lookup"><span data-stu-id="ed7e9-115">gender</span></span>|<span data-ttu-id="ed7e9-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="ed7e9-116">educationGender</span></span>| <span data-ttu-id="ed7e9-117">Os valores possíveis são: `female`, `male`, `other`.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-117">Possible values are: `female`, `male`, `other`.</span></span>|
|<span data-ttu-id="ed7e9-118">grade</span><span class="sxs-lookup"><span data-stu-id="ed7e9-118">grade</span></span>|<span data-ttu-id="ed7e9-119">String</span><span class="sxs-lookup"><span data-stu-id="ed7e9-119">String</span></span>|<span data-ttu-id="ed7e9-120">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="ed7e9-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="ed7e9-121">graduationYear</span></span>|<span data-ttu-id="ed7e9-122">String</span><span class="sxs-lookup"><span data-stu-id="ed7e9-122">String</span></span>| <span data-ttu-id="ed7e9-123">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="ed7e9-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="ed7e9-124">studentNumber</span></span>|<span data-ttu-id="ed7e9-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed7e9-125">String</span></span>| <span data-ttu-id="ed7e9-126">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed7e9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed7e9-127">JSON representation</span></span>

<span data-ttu-id="ed7e9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed7e9-128">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
