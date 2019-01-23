---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ce3e28ccedc5f6165c8c333afb2ccd10343f14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406903"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="56fd1-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="56fd1-103">educationStudent resource type</span></span>

> <span data-ttu-id="56fd1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="56fd1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56fd1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="56fd1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56fd1-106">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="56fd1-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="56fd1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56fd1-107">Properties</span></span>
| <span data-ttu-id="56fd1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56fd1-108">Property</span></span>     | <span data-ttu-id="56fd1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="56fd1-109">Type</span></span>   |<span data-ttu-id="56fd1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="56fd1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56fd1-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="56fd1-111">birthDate</span></span>|<span data-ttu-id="56fd1-112">Data</span><span class="sxs-lookup"><span data-stu-id="56fd1-112">Date</span></span>| <span data-ttu-id="56fd1-113">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="56fd1-113">Birth date of the student.</span></span>|
|<span data-ttu-id="56fd1-114">externalId</span><span class="sxs-lookup"><span data-stu-id="56fd1-114">externalId</span></span>|<span data-ttu-id="56fd1-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56fd1-115">String</span></span>| <span data-ttu-id="56fd1-116">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="56fd1-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="56fd1-117">gender</span><span class="sxs-lookup"><span data-stu-id="56fd1-117">gender</span></span>|<span data-ttu-id="56fd1-118">educationGender</span><span class="sxs-lookup"><span data-stu-id="56fd1-118">educationGender</span></span>| <span data-ttu-id="56fd1-119">Os valores possíveis são: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="56fd1-119">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="56fd1-120">grade</span><span class="sxs-lookup"><span data-stu-id="56fd1-120">grade</span></span>|<span data-ttu-id="56fd1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56fd1-121">String</span></span>|<span data-ttu-id="56fd1-122">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="56fd1-122">Current grade level of the student.</span></span>|
|<span data-ttu-id="56fd1-123">graduationYear</span><span class="sxs-lookup"><span data-stu-id="56fd1-123">graduationYear</span></span>|<span data-ttu-id="56fd1-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56fd1-124">String</span></span>| <span data-ttu-id="56fd1-125">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="56fd1-125">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="56fd1-126">studentNumber</span><span class="sxs-lookup"><span data-stu-id="56fd1-126">studentNumber</span></span>|<span data-ttu-id="56fd1-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56fd1-127">String</span></span>| <span data-ttu-id="56fd1-128">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="56fd1-128">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56fd1-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56fd1-129">JSON representation</span></span>

<span data-ttu-id="56fd1-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56fd1-130">The following is a JSON representation of the resource.</span></span>

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
