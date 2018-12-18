---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
ms.openlocfilehash: ce84c9f6abb71e99bf3d886e5bad9e7e97bcb513
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313080"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="2752d-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="2752d-103">educationStudent resource type</span></span>

> <span data-ttu-id="2752d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2752d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2752d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2752d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2752d-106">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="2752d-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="2752d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2752d-107">Properties</span></span>
| <span data-ttu-id="2752d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2752d-108">Property</span></span>     | <span data-ttu-id="2752d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2752d-109">Type</span></span>   |<span data-ttu-id="2752d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2752d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2752d-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="2752d-111">birthDate</span></span>|<span data-ttu-id="2752d-112">Data</span><span class="sxs-lookup"><span data-stu-id="2752d-112">Date</span></span>| <span data-ttu-id="2752d-113">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="2752d-113">Birth date of the student.</span></span>|
|<span data-ttu-id="2752d-114">externalId</span><span class="sxs-lookup"><span data-stu-id="2752d-114">externalId</span></span>|<span data-ttu-id="2752d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2752d-115">String</span></span>| <span data-ttu-id="2752d-116">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="2752d-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="2752d-117">gender</span><span class="sxs-lookup"><span data-stu-id="2752d-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="2752d-118">Os valores possíveis são: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2752d-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="2752d-119">grade</span><span class="sxs-lookup"><span data-stu-id="2752d-119">grade</span></span>|<span data-ttu-id="2752d-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2752d-120">String</span></span>|<span data-ttu-id="2752d-121">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="2752d-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="2752d-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="2752d-122">graduationYear</span></span>|<span data-ttu-id="2752d-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2752d-123">String</span></span>| <span data-ttu-id="2752d-124">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="2752d-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="2752d-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="2752d-125">studentNumber</span></span>|<span data-ttu-id="2752d-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2752d-126">String</span></span>| <span data-ttu-id="2752d-127">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="2752d-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2752d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2752d-128">JSON representation</span></span>

<span data-ttu-id="2752d-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2752d-129">The following is a JSON representation of the resource.</span></span>

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