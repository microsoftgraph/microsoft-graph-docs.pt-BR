---
title: tipo de recurso personInterest
description: tipo de recurso personInterest
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 05918edf82712d5253403ed63312eb941be14103
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949495"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="6e90f-103">tipo de recurso personInterest</span><span class="sxs-lookup"><span data-stu-id="6e90f-103">personInterest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e90f-104">Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="6e90f-104">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="6e90f-105">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="6e90f-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6e90f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e90f-106">Methods</span></span>

| <span data-ttu-id="6e90f-107">Método</span><span class="sxs-lookup"><span data-stu-id="6e90f-107">Method</span></span>       | <span data-ttu-id="6e90f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e90f-108">Return Type</span></span> | <span data-ttu-id="6e90f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e90f-109">Description</span></span> |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [<span data-ttu-id="6e90f-110">Obter personInterest</span><span class="sxs-lookup"><span data-stu-id="6e90f-110">Get personInterest</span></span>](../api/personinterest-get.md) | [<span data-ttu-id="6e90f-111">personInterest</span><span class="sxs-lookup"><span data-stu-id="6e90f-111">personInterest</span></span>](personinterest.md) | <span data-ttu-id="6e90f-112">Leia as propriedades e os relacionamentos de um objeto **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="6e90f-112">Read the properties and relationships of a **personInterest** object.</span></span> |
| [<span data-ttu-id="6e90f-113">Atualizar personInterest</span><span class="sxs-lookup"><span data-stu-id="6e90f-113">Update personInterest</span></span>](../api/personinterest-update.md)          | [<span data-ttu-id="6e90f-114">personInterest</span><span class="sxs-lookup"><span data-stu-id="6e90f-114">personInterest</span></span>](personinterest.md) | <span data-ttu-id="6e90f-115">Atualizar um objeto **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="6e90f-115">Update a **personInterest** object.</span></span>                               |
| [<span data-ttu-id="6e90f-116">Excluir personInterest</span><span class="sxs-lookup"><span data-stu-id="6e90f-116">Delete personInterest</span></span>](../api/personinterest-delete.md)          | <span data-ttu-id="6e90f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e90f-117">None</span></span>                                | <span data-ttu-id="6e90f-118">Excluir um objeto **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="6e90f-118">Delete a **personInterest** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="6e90f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e90f-119">Properties</span></span>

| <span data-ttu-id="6e90f-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e90f-120">Property</span></span>     | <span data-ttu-id="6e90f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e90f-121">Type</span></span>             | <span data-ttu-id="6e90f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e90f-122">Description</span></span>                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|<span data-ttu-id="6e90f-123">categories</span><span class="sxs-lookup"><span data-stu-id="6e90f-123">categories</span></span>    |<span data-ttu-id="6e90f-124">String collection</span><span class="sxs-lookup"><span data-stu-id="6e90f-124">String collection</span></span> | <span data-ttu-id="6e90f-125">Contém categorias que um usuário associou aos juros (por exemplo, pessoal, recipies).</span><span class="sxs-lookup"><span data-stu-id="6e90f-125">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="6e90f-126">description</span><span class="sxs-lookup"><span data-stu-id="6e90f-126">description</span></span>   |<span data-ttu-id="6e90f-127">String</span><span class="sxs-lookup"><span data-stu-id="6e90f-127">String</span></span>            | <span data-ttu-id="6e90f-128">Contém uma descrição dos juros.</span><span class="sxs-lookup"><span data-stu-id="6e90f-128">Contains a description of the interest.</span></span>                                              |
|<span data-ttu-id="6e90f-129">displayName</span><span class="sxs-lookup"><span data-stu-id="6e90f-129">displayName</span></span>   |<span data-ttu-id="6e90f-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e90f-130">String</span></span>            | <span data-ttu-id="6e90f-131">Contém um nome amigável para os juros.</span><span class="sxs-lookup"><span data-stu-id="6e90f-131">Contains a friendly name for the interest.</span></span>                                           |
|<span data-ttu-id="6e90f-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="6e90f-132">webUrl</span></span>        |<span data-ttu-id="6e90f-133">String</span><span class="sxs-lookup"><span data-stu-id="6e90f-133">String</span></span>            | <span data-ttu-id="6e90f-134">Contém um link para uma página da Web ou recurso sobre os juros.</span><span class="sxs-lookup"><span data-stu-id="6e90f-134">Contains a link to a web page or resource about the interest.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="6e90f-135">Relações</span><span class="sxs-lookup"><span data-stu-id="6e90f-135">Relationships</span></span>

<span data-ttu-id="6e90f-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e90f-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e90f-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e90f-137">JSON representation</span></span>

<span data-ttu-id="6e90f-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e90f-138">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personInterest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
