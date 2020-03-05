---
title: tipo de recurso skillProficiency
description: tipo de recurso skillProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6662ab205e390ae72d283d5015aa346c4b6fc2b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520503"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="eb3d9-103">tipo de recurso skillProficiency</span><span class="sxs-lookup"><span data-stu-id="eb3d9-103">skillProficiency resource type</span></span>

<span data-ttu-id="eb3d9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb3d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb3d9-105">Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="eb3d9-105">Represents detailed information about skills associated with a user in various services.</span></span>

<span data-ttu-id="eb3d9-106">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="eb3d9-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eb3d9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb3d9-107">Methods</span></span>
 
| <span data-ttu-id="eb3d9-108">Método</span><span class="sxs-lookup"><span data-stu-id="eb3d9-108">Method</span></span>                                                 | <span data-ttu-id="eb3d9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb3d9-109">Return Type</span></span>                             | <span data-ttu-id="eb3d9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb3d9-110">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="eb3d9-111">Obter skillProficiency</span><span class="sxs-lookup"><span data-stu-id="eb3d9-111">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="eb3d9-112">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="eb3d9-112">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="eb3d9-113">Leia as propriedades e os relacionamentos de um objeto **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="eb3d9-113">Read the properties and relationships of a **skillProficiency** object.</span></span> |
| [<span data-ttu-id="eb3d9-114">Atualizar skillProficiency</span><span class="sxs-lookup"><span data-stu-id="eb3d9-114">Update skillProficiency</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="eb3d9-115">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="eb3d9-115">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="eb3d9-116">Atualizar um objeto **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="eb3d9-116">Update a **skillProficiency** object.</span></span>                               |
| [<span data-ttu-id="eb3d9-117">Excluir skillProficiency</span><span class="sxs-lookup"><span data-stu-id="eb3d9-117">Delete skillProficiency</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="eb3d9-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb3d9-118">None</span></span>                                    | <span data-ttu-id="eb3d9-119">Excluir um objeto **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="eb3d9-119">Delete a **skillProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="eb3d9-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb3d9-120">Properties</span></span>

| <span data-ttu-id="eb3d9-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb3d9-121">Property</span></span>     | <span data-ttu-id="eb3d9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb3d9-122">Type</span></span>             | <span data-ttu-id="eb3d9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb3d9-123">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="eb3d9-124">categories</span><span class="sxs-lookup"><span data-stu-id="eb3d9-124">categories</span></span>    |<span data-ttu-id="eb3d9-125">String collection</span><span class="sxs-lookup"><span data-stu-id="eb3d9-125">String collection</span></span> | <span data-ttu-id="eb3d9-126">Contém categorias que um usuário associou à habilidade (por exemplo, pessoal, profissional, hobby).</span><span class="sxs-lookup"><span data-stu-id="eb3d9-126">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span>                                       |
|<span data-ttu-id="eb3d9-127">displayName</span><span class="sxs-lookup"><span data-stu-id="eb3d9-127">displayName</span></span>   |<span data-ttu-id="eb3d9-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb3d9-128">String</span></span>            | <span data-ttu-id="eb3d9-129">Contém um nome amigável para a habilidade.</span><span class="sxs-lookup"><span data-stu-id="eb3d9-129">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="eb3d9-130">proficiência</span><span class="sxs-lookup"><span data-stu-id="eb3d9-130">proficiency</span></span>   |<span data-ttu-id="eb3d9-131">string</span><span class="sxs-lookup"><span data-stu-id="eb3d9-131">string</span></span>            | <span data-ttu-id="eb3d9-132">Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="eb3d9-132">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="eb3d9-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="eb3d9-133">webUrl</span></span>        |<span data-ttu-id="eb3d9-134">String</span><span class="sxs-lookup"><span data-stu-id="eb3d9-134">String</span></span>            | <span data-ttu-id="eb3d9-135">Contém um link para uma fonte de informações sobre a habilidade.</span><span class="sxs-lookup"><span data-stu-id="eb3d9-135">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="eb3d9-136">Relações</span><span class="sxs-lookup"><span data-stu-id="eb3d9-136">Relationships</span></span>

<span data-ttu-id="eb3d9-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb3d9-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb3d9-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb3d9-138">JSON representation</span></span>

<span data-ttu-id="eb3d9-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb3d9-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "displayName": "String",
  "proficiency": "string",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "skillProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
