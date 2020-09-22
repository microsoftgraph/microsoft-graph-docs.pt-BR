---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 355230339129a351f5a609292e7e7623a39a59b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049728"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="67fee-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="67fee-103">educationStudent resource type</span></span>

<span data-ttu-id="67fee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67fee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67fee-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="67fee-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="67fee-106">Ao usar escopos de permissão delegada, o Graph retornará apenas as `externalId` Propriedades.</span><span class="sxs-lookup"><span data-stu-id="67fee-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="67fee-107">Todas as outras propriedades exigem escopos de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="67fee-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="67fee-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67fee-108">Properties</span></span>

| <span data-ttu-id="67fee-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67fee-109">Property</span></span>       | <span data-ttu-id="67fee-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="67fee-110">Type</span></span>            | <span data-ttu-id="67fee-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67fee-111">Description</span></span>                                     |
| :------------- | :-------------- | :---------------------------------------------- |
| <span data-ttu-id="67fee-112">birthDate</span><span class="sxs-lookup"><span data-stu-id="67fee-112">birthDate</span></span>      | <span data-ttu-id="67fee-113">Data</span><span class="sxs-lookup"><span data-stu-id="67fee-113">Date</span></span>            | <span data-ttu-id="67fee-114">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="67fee-114">Birth date of the student.</span></span>                      |
| <span data-ttu-id="67fee-115">externalId</span><span class="sxs-lookup"><span data-stu-id="67fee-115">externalId</span></span>     | <span data-ttu-id="67fee-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67fee-116">String</span></span>          | <span data-ttu-id="67fee-117">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="67fee-117">ID of the student in the source system.</span></span>         |
| <span data-ttu-id="67fee-118">gender</span><span class="sxs-lookup"><span data-stu-id="67fee-118">gender</span></span>         | <span data-ttu-id="67fee-119">educationGender</span><span class="sxs-lookup"><span data-stu-id="67fee-119">educationGender</span></span> | <span data-ttu-id="67fee-120">Os valores possíveis são: `female`, `male`, `other`.</span><span class="sxs-lookup"><span data-stu-id="67fee-120">Possible values are: `female`, `male`, `other`.</span></span> |
| <span data-ttu-id="67fee-121">grade</span><span class="sxs-lookup"><span data-stu-id="67fee-121">grade</span></span>          | <span data-ttu-id="67fee-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67fee-122">String</span></span>          | <span data-ttu-id="67fee-123">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="67fee-123">Current grade level of the student.</span></span>             |
| <span data-ttu-id="67fee-124">graduationYear</span><span class="sxs-lookup"><span data-stu-id="67fee-124">graduationYear</span></span> | <span data-ttu-id="67fee-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67fee-125">String</span></span>          | <span data-ttu-id="67fee-126">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="67fee-126">Year the student is graduating from the school.</span></span> |
| <span data-ttu-id="67fee-127">studentNumber</span><span class="sxs-lookup"><span data-stu-id="67fee-127">studentNumber</span></span>  | <span data-ttu-id="67fee-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67fee-128">String</span></span>          | <span data-ttu-id="67fee-129">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="67fee-129">Student Number.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="67fee-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67fee-130">JSON representation</span></span>

<span data-ttu-id="67fee-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67fee-131">The following is a JSON representation of the resource.</span></span>

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


