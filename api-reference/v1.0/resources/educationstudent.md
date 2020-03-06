---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b9d98d64dbb5e859f98eca84bb46a3137d808424
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531495"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="08963-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="08963-103">educationStudent resource type</span></span>

<span data-ttu-id="08963-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08963-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08963-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="08963-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="08963-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08963-106">Properties</span></span>
| <span data-ttu-id="08963-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08963-107">Property</span></span>     | <span data-ttu-id="08963-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="08963-108">Type</span></span>   |<span data-ttu-id="08963-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08963-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08963-110">birthDate</span><span class="sxs-lookup"><span data-stu-id="08963-110">birthDate</span></span>|<span data-ttu-id="08963-111">Data</span><span class="sxs-lookup"><span data-stu-id="08963-111">Date</span></span>| <span data-ttu-id="08963-112">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="08963-112">Birth date of the student.</span></span>|
|<span data-ttu-id="08963-113">externalId</span><span class="sxs-lookup"><span data-stu-id="08963-113">externalId</span></span>|<span data-ttu-id="08963-114">String</span><span class="sxs-lookup"><span data-stu-id="08963-114">String</span></span>| <span data-ttu-id="08963-115">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="08963-115">ID of the student in the source system.</span></span>|
|<span data-ttu-id="08963-116">gender</span><span class="sxs-lookup"><span data-stu-id="08963-116">gender</span></span>|<span data-ttu-id="08963-117">educationGender</span><span class="sxs-lookup"><span data-stu-id="08963-117">educationGender</span></span>| <span data-ttu-id="08963-118">Os valores possíveis são: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="08963-118">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="08963-119">grade</span><span class="sxs-lookup"><span data-stu-id="08963-119">grade</span></span>|<span data-ttu-id="08963-120">String</span><span class="sxs-lookup"><span data-stu-id="08963-120">String</span></span>|<span data-ttu-id="08963-121">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="08963-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="08963-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="08963-122">graduationYear</span></span>|<span data-ttu-id="08963-123">String</span><span class="sxs-lookup"><span data-stu-id="08963-123">String</span></span>| <span data-ttu-id="08963-124">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="08963-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="08963-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="08963-125">studentNumber</span></span>|<span data-ttu-id="08963-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08963-126">String</span></span>| <span data-ttu-id="08963-127">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="08963-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08963-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08963-128">JSON representation</span></span>

<span data-ttu-id="08963-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08963-129">The following is a JSON representation of the resource.</span></span>

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
