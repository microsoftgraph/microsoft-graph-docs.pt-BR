---
title: tipo de recurso skillProficiency
description: tipo de recurso skillProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0bb63903b5a3eb0eeed8683463b9927537180f53
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950420"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="cbec3-103">tipo de recurso skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cbec3-103">skillProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbec3-104">Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="cbec3-104">Represents detailed information about skills associated with a user in various services.</span></span>

<span data-ttu-id="cbec3-105">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cbec3-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cbec3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cbec3-106">Methods</span></span>
 
| <span data-ttu-id="cbec3-107">Método</span><span class="sxs-lookup"><span data-stu-id="cbec3-107">Method</span></span>                                                 | <span data-ttu-id="cbec3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cbec3-108">Return Type</span></span>                             | <span data-ttu-id="cbec3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbec3-109">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="cbec3-110">Obter skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cbec3-110">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="cbec3-111">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cbec3-111">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="cbec3-112">Leia as propriedades e os relacionamentos de um objeto **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="cbec3-112">Read the properties and relationships of a **skillProficiency** object.</span></span> |
| [<span data-ttu-id="cbec3-113">Atualizar skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cbec3-113">Update skillProficiency</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="cbec3-114">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cbec3-114">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="cbec3-115">Atualizar um objeto **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="cbec3-115">Update a **skillProficiency** object.</span></span>                               |
| [<span data-ttu-id="cbec3-116">Excluir skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cbec3-116">Delete skillProficiency</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="cbec3-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbec3-117">None</span></span>                                    | <span data-ttu-id="cbec3-118">Excluir um objeto **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="cbec3-118">Delete a **skillProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="cbec3-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbec3-119">Properties</span></span>

| <span data-ttu-id="cbec3-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbec3-120">Property</span></span>     | <span data-ttu-id="cbec3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbec3-121">Type</span></span>             | <span data-ttu-id="cbec3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbec3-122">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="cbec3-123">categories</span><span class="sxs-lookup"><span data-stu-id="cbec3-123">categories</span></span>    |<span data-ttu-id="cbec3-124">String collection</span><span class="sxs-lookup"><span data-stu-id="cbec3-124">String collection</span></span> | <span data-ttu-id="cbec3-125">Contém categorias que um usuário associou à habilidade (por exemplo, pessoal, profissional, hobby).</span><span class="sxs-lookup"><span data-stu-id="cbec3-125">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span>                                       |
|<span data-ttu-id="cbec3-126">displayName</span><span class="sxs-lookup"><span data-stu-id="cbec3-126">displayName</span></span>   |<span data-ttu-id="cbec3-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbec3-127">String</span></span>            | <span data-ttu-id="cbec3-128">Contém um nome amigável para a habilidade.</span><span class="sxs-lookup"><span data-stu-id="cbec3-128">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="cbec3-129">proficiência</span><span class="sxs-lookup"><span data-stu-id="cbec3-129">proficiency</span></span>   |<span data-ttu-id="cbec3-130">string</span><span class="sxs-lookup"><span data-stu-id="cbec3-130">string</span></span>            | <span data-ttu-id="cbec3-131">Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cbec3-131">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cbec3-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="cbec3-132">webUrl</span></span>        |<span data-ttu-id="cbec3-133">String</span><span class="sxs-lookup"><span data-stu-id="cbec3-133">String</span></span>            | <span data-ttu-id="cbec3-134">Contém um link para uma fonte de informações sobre a habilidade.</span><span class="sxs-lookup"><span data-stu-id="cbec3-134">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="cbec3-135">Relações</span><span class="sxs-lookup"><span data-stu-id="cbec3-135">Relationships</span></span>

<span data-ttu-id="cbec3-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbec3-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbec3-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbec3-137">JSON representation</span></span>

<span data-ttu-id="cbec3-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbec3-138">The following is a JSON representation of the resource.</span></span>

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
