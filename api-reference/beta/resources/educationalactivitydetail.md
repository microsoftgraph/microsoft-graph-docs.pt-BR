---
title: tipo de recurso educationalActivityDetail
description: tipo de recurso educationalActivityDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2f19f5e02ae26281a5ac1b2b48498a426f976e8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055656"
---
# <a name="educationalactivitydetail-resource-type"></a><span data-ttu-id="f129c-103">tipo de recurso educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="f129c-103">educationalActivityDetail resource type</span></span>

<span data-ttu-id="f129c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f129c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f129c-105">Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="f129c-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="f129c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f129c-106">Properties</span></span>

| <span data-ttu-id="f129c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f129c-107">Property</span></span>     | <span data-ttu-id="f129c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f129c-108">Type</span></span>        | <span data-ttu-id="f129c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f129c-109">Description</span></span>                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|<span data-ttu-id="f129c-110">abreviação</span><span class="sxs-lookup"><span data-stu-id="f129c-110">abbreviation</span></span>  |<span data-ttu-id="f129c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f129c-111">String</span></span>       |<span data-ttu-id="f129c-112">Nome abreviado do grau ou do programa (exemplo: PhD, MBA)</span><span class="sxs-lookup"><span data-stu-id="f129c-112">Shortened name of the degree or program (example: PhD, MBA)</span></span>    |
|<span data-ttu-id="f129c-113">activities</span><span class="sxs-lookup"><span data-stu-id="f129c-113">activities</span></span>    |<span data-ttu-id="f129c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f129c-114">String</span></span>       |<span data-ttu-id="f129c-115">As atividades do extracurriculares são realizadas junto com o programa.</span><span class="sxs-lookup"><span data-stu-id="f129c-115">Extracurricular activities undertaken alongside the program.</span></span>   |
|<span data-ttu-id="f129c-116">awards</span><span class="sxs-lookup"><span data-stu-id="f129c-116">awards</span></span>        |<span data-ttu-id="f129c-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f129c-117">String</span></span>       |<span data-ttu-id="f129c-118">Quaisquer prêmios ou honras associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="f129c-118">Any awards or honors associated with the program.</span></span>              |
|<span data-ttu-id="f129c-119">description</span><span class="sxs-lookup"><span data-stu-id="f129c-119">description</span></span>   |<span data-ttu-id="f129c-120">String</span><span class="sxs-lookup"><span data-stu-id="f129c-120">String</span></span>       |<span data-ttu-id="f129c-121">Breve descrição do programa fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f129c-121">Short description of the program provided by the user.</span></span>         |
|<span data-ttu-id="f129c-122">displayName</span><span class="sxs-lookup"><span data-stu-id="f129c-122">displayName</span></span>   |<span data-ttu-id="f129c-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f129c-123">String</span></span>       |<span data-ttu-id="f129c-124">Nome de formato longo do programa que o usuário forneceu.</span><span class="sxs-lookup"><span data-stu-id="f129c-124">Long-form name of the program that the user has provided.</span></span>      |
|<span data-ttu-id="f129c-125">fieldsOfStudy</span><span class="sxs-lookup"><span data-stu-id="f129c-125">fieldsOfStudy</span></span> |<span data-ttu-id="f129c-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f129c-126">String</span></span>       |<span data-ttu-id="f129c-127">Principais e menores associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="f129c-127">Majors and minors associated with the program.</span></span> <span data-ttu-id="f129c-128">(se aplicável)</span><span class="sxs-lookup"><span data-stu-id="f129c-128">(if applicable)</span></span> |
|<span data-ttu-id="f129c-129">grade</span><span class="sxs-lookup"><span data-stu-id="f129c-129">grade</span></span>         |<span data-ttu-id="f129c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f129c-130">String</span></span>       |<span data-ttu-id="f129c-131">A classificação final, turma, média ou pontuação.</span><span class="sxs-lookup"><span data-stu-id="f129c-131">The final grade, class, GPA or score.</span></span>                          |
|<span data-ttu-id="f129c-132">notes</span><span class="sxs-lookup"><span data-stu-id="f129c-132">notes</span></span>         |<span data-ttu-id="f129c-133">String</span><span class="sxs-lookup"><span data-stu-id="f129c-133">String</span></span>       |<span data-ttu-id="f129c-134">Observações adicionais que o usuário forneceu.</span><span class="sxs-lookup"><span data-stu-id="f129c-134">Additional notes the user has provided.</span></span>                        |
|<span data-ttu-id="f129c-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="f129c-135">webUrl</span></span>        |<span data-ttu-id="f129c-136">String</span><span class="sxs-lookup"><span data-stu-id="f129c-136">String</span></span>       |<span data-ttu-id="f129c-137">Link para a página de grau ou de programa.</span><span class="sxs-lookup"><span data-stu-id="f129c-137">Link to the degree or program page.</span></span>                            |

## <a name="json-representation"></a><span data-ttu-id="f129c-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f129c-138">JSON representation</span></span>

<span data-ttu-id="f129c-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f129c-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivityDetail",
  "baseType": null
}-->

```json
{
  "abbreviation": "String",
  "activities": "String",
  "awards": "String",
  "description": "String",
  "displayName": "String",
  "fieldsOfStudy": "String",
  "grade": "String",
  "notes": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivityDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

