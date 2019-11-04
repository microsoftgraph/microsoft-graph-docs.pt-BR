---
title: tipo de recurso skillProficiency
description: tipo de recurso skillProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9490947aea170f2b6e94ecd8f02f59d396746e3a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938706"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="00bd8-103">tipo de recurso skillProficiency</span><span class="sxs-lookup"><span data-stu-id="00bd8-103">skillProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00bd8-104">Representa informações detalhadas sobre as habilidades que o usuário tenha associado a si mesmas em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="00bd8-104">Represents detailed information about skills the user has associated with themselves in various services.</span></span>

<span data-ttu-id="00bd8-105">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="00bd8-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="00bd8-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="00bd8-106">Methods</span></span>
 
| <span data-ttu-id="00bd8-107">Método</span><span class="sxs-lookup"><span data-stu-id="00bd8-107">Method</span></span>                                                 | <span data-ttu-id="00bd8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="00bd8-108">Return Type</span></span>                             | <span data-ttu-id="00bd8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bd8-109">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="00bd8-110">Obter skillProficiency</span><span class="sxs-lookup"><span data-stu-id="00bd8-110">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="00bd8-111">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="00bd8-111">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="00bd8-112">Leia as propriedades e os relacionamentos do objeto skillProficiency.</span><span class="sxs-lookup"><span data-stu-id="00bd8-112">Read properties and relationships of skillProficiency object.</span></span> |
| [<span data-ttu-id="00bd8-113">Update</span><span class="sxs-lookup"><span data-stu-id="00bd8-113">Update</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="00bd8-114">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="00bd8-114">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="00bd8-115">Atualize o objeto skillProficiency.</span><span class="sxs-lookup"><span data-stu-id="00bd8-115">Update skillProficiency object.</span></span>                               |
| [<span data-ttu-id="00bd8-116">Delete</span><span class="sxs-lookup"><span data-stu-id="00bd8-116">Delete</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="00bd8-117">None</span><span class="sxs-lookup"><span data-stu-id="00bd8-117">None</span></span>                                    | <span data-ttu-id="00bd8-118">Exclua o objeto skillProficiency.</span><span class="sxs-lookup"><span data-stu-id="00bd8-118">Delete skillProficiency object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="00bd8-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00bd8-119">Properties</span></span>

| <span data-ttu-id="00bd8-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00bd8-120">Property</span></span>     | <span data-ttu-id="00bd8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="00bd8-121">Type</span></span>             | <span data-ttu-id="00bd8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bd8-122">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="00bd8-123">categories</span><span class="sxs-lookup"><span data-stu-id="00bd8-123">categories</span></span>    |<span data-ttu-id="00bd8-124">String collection</span><span class="sxs-lookup"><span data-stu-id="00bd8-124">String collection</span></span> | <span data-ttu-id="00bd8-125">Contém categorias que um usuário associou à habilidade (por exemplo: pessoal, profissional, hobby)</span><span class="sxs-lookup"><span data-stu-id="00bd8-125">Contains categories a user has associated with the skill (eg: personal, professional, hobby)</span></span>                                       |
|<span data-ttu-id="00bd8-126">displayName</span><span class="sxs-lookup"><span data-stu-id="00bd8-126">displayName</span></span>   |<span data-ttu-id="00bd8-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00bd8-127">String</span></span>            | <span data-ttu-id="00bd8-128">Contém um nome amigável para a habilidade.</span><span class="sxs-lookup"><span data-stu-id="00bd8-128">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="00bd8-129">proficiência</span><span class="sxs-lookup"><span data-stu-id="00bd8-129">proficiency</span></span>   |<span data-ttu-id="00bd8-130">string</span><span class="sxs-lookup"><span data-stu-id="00bd8-130">string</span></span>            | <span data-ttu-id="00bd8-131">Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="00bd8-131">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="00bd8-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="00bd8-132">webUrl</span></span>        |<span data-ttu-id="00bd8-133">String</span><span class="sxs-lookup"><span data-stu-id="00bd8-133">String</span></span>            | <span data-ttu-id="00bd8-134">Contém um link para uma fonte de informações sobre a habilidade.</span><span class="sxs-lookup"><span data-stu-id="00bd8-134">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="00bd8-135">Relações</span><span class="sxs-lookup"><span data-stu-id="00bd8-135">Relationships</span></span>

<span data-ttu-id="00bd8-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00bd8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00bd8-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00bd8-137">JSON representation</span></span>

<span data-ttu-id="00bd8-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00bd8-138">The following is a JSON representation of the resource.</span></span>

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