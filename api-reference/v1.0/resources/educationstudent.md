---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b0e154beb5b8133c69392af8fa9611263c68945
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231847"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="68283-103">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="68283-103">educationStudent resource type</span></span>

<span data-ttu-id="68283-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68283-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68283-105">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="68283-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="68283-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68283-106">Properties</span></span>

| <span data-ttu-id="68283-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68283-107">Property</span></span>       | <span data-ttu-id="68283-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="68283-108">Type</span></span>            | <span data-ttu-id="68283-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="68283-109">Description</span></span>                                                               |
| :------------- | :-------------- | :------------------------------------------------------------------------ |
| <span data-ttu-id="68283-110">birthDate</span><span class="sxs-lookup"><span data-stu-id="68283-110">birthDate</span></span>      | <span data-ttu-id="68283-111">Data</span><span class="sxs-lookup"><span data-stu-id="68283-111">Date</span></span>            | <span data-ttu-id="68283-112">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="68283-112">Birth date of the student.</span></span>                                                |
| <span data-ttu-id="68283-113">externalId</span><span class="sxs-lookup"><span data-stu-id="68283-113">externalId</span></span>     | <span data-ttu-id="68283-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68283-114">String</span></span>          | <span data-ttu-id="68283-115">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="68283-115">ID of the student in the source system.</span></span>                                   |
| <span data-ttu-id="68283-116">gender</span><span class="sxs-lookup"><span data-stu-id="68283-116">gender</span></span>         | <span data-ttu-id="68283-117">educationGender</span><span class="sxs-lookup"><span data-stu-id="68283-117">educationGender</span></span> | <span data-ttu-id="68283-118">Os valores possíveis são: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="68283-118">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="68283-119">grade</span><span class="sxs-lookup"><span data-stu-id="68283-119">grade</span></span>          | <span data-ttu-id="68283-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68283-120">String</span></span>          | <span data-ttu-id="68283-121">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="68283-121">Current grade level of the student.</span></span>                                       |
| <span data-ttu-id="68283-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="68283-122">graduationYear</span></span> | <span data-ttu-id="68283-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68283-123">String</span></span>          | <span data-ttu-id="68283-124">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="68283-124">Year the student is graduating from the school.</span></span>                           |
| <span data-ttu-id="68283-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="68283-125">studentNumber</span></span>  | <span data-ttu-id="68283-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68283-126">String</span></span>          | <span data-ttu-id="68283-127">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="68283-127">Student Number.</span></span>                                                           |

## <a name="relationships"></a><span data-ttu-id="68283-128">Relações</span><span class="sxs-lookup"><span data-stu-id="68283-128">Relationships</span></span>

<span data-ttu-id="68283-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68283-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68283-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68283-130">JSON representation</span></span>

<span data-ttu-id="68283-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68283-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "DateTimeOffset",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```
