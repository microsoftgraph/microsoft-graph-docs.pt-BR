---
title: tipo de recurso educationalActivityDetail
description: tipo de recurso educationalActivityDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e8e79ac7831698bf22d5785b83ebaa71961e19df
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935064"
---
# <a name="educationalactivitydetail-resource-type"></a><span data-ttu-id="4e04d-103">tipo de recurso educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="4e04d-103">educationalActivityDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e04d-104">Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="4e04d-104">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="4e04d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e04d-105">Properties</span></span>

| <span data-ttu-id="4e04d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e04d-106">Property</span></span>     | <span data-ttu-id="4e04d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e04d-107">Type</span></span>        | <span data-ttu-id="4e04d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e04d-108">Description</span></span>                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|<span data-ttu-id="4e04d-109">abreviação</span><span class="sxs-lookup"><span data-stu-id="4e04d-109">abbreviation</span></span>  |<span data-ttu-id="4e04d-110">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-110">String</span></span>       |<span data-ttu-id="4e04d-111">Nome abreviado do grau ou do programa (exemplo: PhD, MBA)</span><span class="sxs-lookup"><span data-stu-id="4e04d-111">Shortened name of the degree or program (example: PhD, MBA)</span></span>    |
|<span data-ttu-id="4e04d-112">activities</span><span class="sxs-lookup"><span data-stu-id="4e04d-112">activities</span></span>    |<span data-ttu-id="4e04d-113">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-113">String</span></span>       |<span data-ttu-id="4e04d-114">As atividades do extracurriculares são realizadas junto com o programa.</span><span class="sxs-lookup"><span data-stu-id="4e04d-114">Extracurricular activities undertaken alongside the program.</span></span>   |
|<span data-ttu-id="4e04d-115">concede</span><span class="sxs-lookup"><span data-stu-id="4e04d-115">awards</span></span>        |<span data-ttu-id="4e04d-116">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-116">String</span></span>       |<span data-ttu-id="4e04d-117">Quaisquer prêmios ou honras associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="4e04d-117">Any awards or honors associated with the program.</span></span>              |
|<span data-ttu-id="4e04d-118">description</span><span class="sxs-lookup"><span data-stu-id="4e04d-118">description</span></span>   |<span data-ttu-id="4e04d-119">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-119">String</span></span>       |<span data-ttu-id="4e04d-120">Breve descrição do programa fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="4e04d-120">Short description of the program provided by the user.</span></span>         |
|<span data-ttu-id="4e04d-121">displayName</span><span class="sxs-lookup"><span data-stu-id="4e04d-121">displayName</span></span>   |<span data-ttu-id="4e04d-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e04d-122">String</span></span>       |<span data-ttu-id="4e04d-123">Nome de formato longo do programa que o usuário forneceu.</span><span class="sxs-lookup"><span data-stu-id="4e04d-123">Long-form name of the program that the user has provided.</span></span>      |
|<span data-ttu-id="4e04d-124">fieldsOfStudy</span><span class="sxs-lookup"><span data-stu-id="4e04d-124">fieldsOfStudy</span></span> |<span data-ttu-id="4e04d-125">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-125">String</span></span>       |<span data-ttu-id="4e04d-126">Principais e menores associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="4e04d-126">Majors and minors associated with the program.</span></span> <span data-ttu-id="4e04d-127">(se aplicável)</span><span class="sxs-lookup"><span data-stu-id="4e04d-127">(if applicable)</span></span> |
|<span data-ttu-id="4e04d-128">grade</span><span class="sxs-lookup"><span data-stu-id="4e04d-128">grade</span></span>         |<span data-ttu-id="4e04d-129">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-129">String</span></span>       |<span data-ttu-id="4e04d-130">A classificação final, turma, média ou pontuação.</span><span class="sxs-lookup"><span data-stu-id="4e04d-130">The final grade, class, GPA or score.</span></span>                          |
|<span data-ttu-id="4e04d-131">notes</span><span class="sxs-lookup"><span data-stu-id="4e04d-131">notes</span></span>         |<span data-ttu-id="4e04d-132">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-132">String</span></span>       |<span data-ttu-id="4e04d-133">Observações adicionais que o usuário forneceu.</span><span class="sxs-lookup"><span data-stu-id="4e04d-133">Additional notes the user has provided.</span></span>                        |
|<span data-ttu-id="4e04d-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="4e04d-134">webUrl</span></span>        |<span data-ttu-id="4e04d-135">String</span><span class="sxs-lookup"><span data-stu-id="4e04d-135">String</span></span>       |<span data-ttu-id="4e04d-136">Link para a página de grau ou de programa.</span><span class="sxs-lookup"><span data-stu-id="4e04d-136">Link to the degree or program page.</span></span>                            |

## <a name="json-representation"></a><span data-ttu-id="4e04d-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e04d-137">JSON representation</span></span>

<span data-ttu-id="4e04d-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e04d-138">The following is a JSON representation of the resource.</span></span>

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