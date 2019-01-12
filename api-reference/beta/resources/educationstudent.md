---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b6f6cf8e8a79c427403c2f2157228c8ce130b313
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913307"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="61459-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="61459-103">educationStudent resource type</span></span>

> <span data-ttu-id="61459-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61459-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61459-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61459-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61459-106">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="61459-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="61459-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61459-107">Properties</span></span>
| <span data-ttu-id="61459-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61459-108">Property</span></span>     | <span data-ttu-id="61459-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="61459-109">Type</span></span>   |<span data-ttu-id="61459-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61459-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61459-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="61459-111">birthDate</span></span>|<span data-ttu-id="61459-112">Data</span><span class="sxs-lookup"><span data-stu-id="61459-112">Date</span></span>| <span data-ttu-id="61459-113">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="61459-113">Birth date of the student.</span></span>|
|<span data-ttu-id="61459-114">externalId</span><span class="sxs-lookup"><span data-stu-id="61459-114">externalId</span></span>|<span data-ttu-id="61459-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61459-115">String</span></span>| <span data-ttu-id="61459-116">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="61459-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="61459-117">gender</span><span class="sxs-lookup"><span data-stu-id="61459-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="61459-118">Os valores possíveis são: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="61459-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="61459-119">grade</span><span class="sxs-lookup"><span data-stu-id="61459-119">grade</span></span>|<span data-ttu-id="61459-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61459-120">String</span></span>|<span data-ttu-id="61459-121">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="61459-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="61459-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="61459-122">graduationYear</span></span>|<span data-ttu-id="61459-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61459-123">String</span></span>| <span data-ttu-id="61459-124">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="61459-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="61459-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="61459-125">studentNumber</span></span>|<span data-ttu-id="61459-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61459-126">String</span></span>| <span data-ttu-id="61459-127">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="61459-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61459-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61459-128">JSON representation</span></span>

<span data-ttu-id="61459-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61459-129">The following is a JSON representation of the resource.</span></span>

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
