---
title: tipo de recurso educationalActivityDetail
description: tipo de recurso educationalActivityDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ccacf02184bbf54e49949d7671d34dde93b3859f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502820"
---
# <a name="educationalactivitydetail-resource-type"></a><span data-ttu-id="3e798-103">tipo de recurso educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="3e798-103">educationalActivityDetail resource type</span></span>

<span data-ttu-id="3e798-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3e798-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e798-105">Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="3e798-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3e798-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e798-106">Properties</span></span>

| <span data-ttu-id="3e798-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e798-107">Property</span></span>     | <span data-ttu-id="3e798-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e798-108">Type</span></span>        | <span data-ttu-id="3e798-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e798-109">Description</span></span>                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|<span data-ttu-id="3e798-110">abreviação</span><span class="sxs-lookup"><span data-stu-id="3e798-110">abbreviation</span></span>  |<span data-ttu-id="3e798-111">String</span><span class="sxs-lookup"><span data-stu-id="3e798-111">String</span></span>       |<span data-ttu-id="3e798-112">Nome abreviado do grau ou do programa (exemplo: PhD, MBA)</span><span class="sxs-lookup"><span data-stu-id="3e798-112">Shortened name of the degree or program (example: PhD, MBA)</span></span>    |
|<span data-ttu-id="3e798-113">activities</span><span class="sxs-lookup"><span data-stu-id="3e798-113">activities</span></span>    |<span data-ttu-id="3e798-114">String</span><span class="sxs-lookup"><span data-stu-id="3e798-114">String</span></span>       |<span data-ttu-id="3e798-115">As atividades do extracurriculares são realizadas junto com o programa.</span><span class="sxs-lookup"><span data-stu-id="3e798-115">Extracurricular activities undertaken alongside the program.</span></span>   |
|<span data-ttu-id="3e798-116">concede</span><span class="sxs-lookup"><span data-stu-id="3e798-116">awards</span></span>        |<span data-ttu-id="3e798-117">String</span><span class="sxs-lookup"><span data-stu-id="3e798-117">String</span></span>       |<span data-ttu-id="3e798-118">Quaisquer prêmios ou honras associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="3e798-118">Any awards or honors associated with the program.</span></span>              |
|<span data-ttu-id="3e798-119">description</span><span class="sxs-lookup"><span data-stu-id="3e798-119">description</span></span>   |<span data-ttu-id="3e798-120">String</span><span class="sxs-lookup"><span data-stu-id="3e798-120">String</span></span>       |<span data-ttu-id="3e798-121">Breve descrição do programa fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3e798-121">Short description of the program provided by the user.</span></span>         |
|<span data-ttu-id="3e798-122">displayName</span><span class="sxs-lookup"><span data-stu-id="3e798-122">displayName</span></span>   |<span data-ttu-id="3e798-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e798-123">String</span></span>       |<span data-ttu-id="3e798-124">Nome de formato longo do programa que o usuário forneceu.</span><span class="sxs-lookup"><span data-stu-id="3e798-124">Long-form name of the program that the user has provided.</span></span>      |
|<span data-ttu-id="3e798-125">fieldsOfStudy</span><span class="sxs-lookup"><span data-stu-id="3e798-125">fieldsOfStudy</span></span> |<span data-ttu-id="3e798-126">String</span><span class="sxs-lookup"><span data-stu-id="3e798-126">String</span></span>       |<span data-ttu-id="3e798-127">Principais e menores associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="3e798-127">Majors and minors associated with the program.</span></span> <span data-ttu-id="3e798-128">(se aplicável)</span><span class="sxs-lookup"><span data-stu-id="3e798-128">(if applicable)</span></span> |
|<span data-ttu-id="3e798-129">grade</span><span class="sxs-lookup"><span data-stu-id="3e798-129">grade</span></span>         |<span data-ttu-id="3e798-130">String</span><span class="sxs-lookup"><span data-stu-id="3e798-130">String</span></span>       |<span data-ttu-id="3e798-131">A classificação final, turma, média ou pontuação.</span><span class="sxs-lookup"><span data-stu-id="3e798-131">The final grade, class, GPA or score.</span></span>                          |
|<span data-ttu-id="3e798-132">notes</span><span class="sxs-lookup"><span data-stu-id="3e798-132">notes</span></span>         |<span data-ttu-id="3e798-133">String</span><span class="sxs-lookup"><span data-stu-id="3e798-133">String</span></span>       |<span data-ttu-id="3e798-134">Observações adicionais que o usuário forneceu.</span><span class="sxs-lookup"><span data-stu-id="3e798-134">Additional notes the user has provided.</span></span>                        |
|<span data-ttu-id="3e798-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="3e798-135">webUrl</span></span>        |<span data-ttu-id="3e798-136">String</span><span class="sxs-lookup"><span data-stu-id="3e798-136">String</span></span>       |<span data-ttu-id="3e798-137">Link para a página de grau ou de programa.</span><span class="sxs-lookup"><span data-stu-id="3e798-137">Link to the degree or program page.</span></span>                            |

## <a name="json-representation"></a><span data-ttu-id="3e798-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e798-138">JSON representation</span></span>

<span data-ttu-id="3e798-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e798-139">The following is a JSON representation of the resource.</span></span>

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