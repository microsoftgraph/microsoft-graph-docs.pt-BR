---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e64899cf56140246373c36428518ebd28bb136c7
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909720"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="971bd-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="971bd-103">educationStudent resource type</span></span>

<span data-ttu-id="971bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="971bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="971bd-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="971bd-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="971bd-106">Ao usar escopos de permissão delegada, o Graph retornará apenas as `externalId` Propriedades.</span><span class="sxs-lookup"><span data-stu-id="971bd-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="971bd-107">Todas as outras propriedades exigem escopos de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="971bd-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="971bd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="971bd-108">Properties</span></span>

| <span data-ttu-id="971bd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="971bd-109">Property</span></span>       | <span data-ttu-id="971bd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="971bd-110">Type</span></span>            | <span data-ttu-id="971bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="971bd-111">Description</span></span>                                     |
| :------------- | :-------------- | :---------------------------------------------- |
| <span data-ttu-id="971bd-112">birthDate</span><span class="sxs-lookup"><span data-stu-id="971bd-112">birthDate</span></span>      | <span data-ttu-id="971bd-113">Data</span><span class="sxs-lookup"><span data-stu-id="971bd-113">Date</span></span>            | <span data-ttu-id="971bd-114">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="971bd-114">Birth date of the student.</span></span>                      |
| <span data-ttu-id="971bd-115">externalId</span><span class="sxs-lookup"><span data-stu-id="971bd-115">externalId</span></span>     | <span data-ttu-id="971bd-116">String</span><span class="sxs-lookup"><span data-stu-id="971bd-116">String</span></span>          | <span data-ttu-id="971bd-117">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="971bd-117">ID of the student in the source system.</span></span>         |
| <span data-ttu-id="971bd-118">gender</span><span class="sxs-lookup"><span data-stu-id="971bd-118">gender</span></span>         | <span data-ttu-id="971bd-119">educationGender</span><span class="sxs-lookup"><span data-stu-id="971bd-119">educationGender</span></span> | <span data-ttu-id="971bd-120">Os valores possíveis são: `female`, `male`, `other`.</span><span class="sxs-lookup"><span data-stu-id="971bd-120">Possible values are: `female`, `male`, `other`.</span></span> |
| <span data-ttu-id="971bd-121">grade</span><span class="sxs-lookup"><span data-stu-id="971bd-121">grade</span></span>          | <span data-ttu-id="971bd-122">String</span><span class="sxs-lookup"><span data-stu-id="971bd-122">String</span></span>          | <span data-ttu-id="971bd-123">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="971bd-123">Current grade level of the student.</span></span>             |
| <span data-ttu-id="971bd-124">graduationYear</span><span class="sxs-lookup"><span data-stu-id="971bd-124">graduationYear</span></span> | <span data-ttu-id="971bd-125">String</span><span class="sxs-lookup"><span data-stu-id="971bd-125">String</span></span>          | <span data-ttu-id="971bd-126">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="971bd-126">Year the student is graduating from the school.</span></span> |
| <span data-ttu-id="971bd-127">studentNumber</span><span class="sxs-lookup"><span data-stu-id="971bd-127">studentNumber</span></span>  | <span data-ttu-id="971bd-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="971bd-128">String</span></span>          | <span data-ttu-id="971bd-129">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="971bd-129">Student Number.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="971bd-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="971bd-130">JSON representation</span></span>

<span data-ttu-id="971bd-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="971bd-131">The following is a JSON representation of the resource.</span></span>

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
