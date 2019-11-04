---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b5e6b8c3013c647087ab3d8db28b0196d0c79036
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949493"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="af1b9-103">tipo de recurso personWebsite</span><span class="sxs-lookup"><span data-stu-id="af1b9-103">personWebsite resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af1b9-104">Representa informações detalhadas sobre sites associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="af1b9-104">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="af1b9-105">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="af1b9-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="af1b9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="af1b9-106">Methods</span></span>

| <span data-ttu-id="af1b9-107">Método</span><span class="sxs-lookup"><span data-stu-id="af1b9-107">Method</span></span>                                           | <span data-ttu-id="af1b9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="af1b9-108">Return Type</span></span>                       | <span data-ttu-id="af1b9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af1b9-109">Description</span></span>                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [<span data-ttu-id="af1b9-110">Obter personWebsite</span><span class="sxs-lookup"><span data-stu-id="af1b9-110">Get personWebsite</span></span>](../api/personwebsite-get.md) | [<span data-ttu-id="af1b9-111">personWebsite</span><span class="sxs-lookup"><span data-stu-id="af1b9-111">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="af1b9-112">Leia as propriedades e os relacionamentos de um objeto **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="af1b9-112">Read the properties and relationships of a **personWebsite** object.</span></span> |
| [<span data-ttu-id="af1b9-113">Atualizar personWebsite</span><span class="sxs-lookup"><span data-stu-id="af1b9-113">Update personWebsite</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="af1b9-114">personWebsite</span><span class="sxs-lookup"><span data-stu-id="af1b9-114">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="af1b9-115">Atualizar um objeto **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="af1b9-115">Update a **personWebsite** object.</span></span>                               |
| [<span data-ttu-id="af1b9-116">Excluir personWebsite</span><span class="sxs-lookup"><span data-stu-id="af1b9-116">Delete personWebsite</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="af1b9-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af1b9-117">None</span></span>                              | <span data-ttu-id="af1b9-118">Excluir um objeto **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="af1b9-118">Delete a **personWebsite** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="af1b9-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af1b9-119">Properties</span></span>

| <span data-ttu-id="af1b9-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af1b9-120">Property</span></span>     | <span data-ttu-id="af1b9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="af1b9-121">Type</span></span>              | <span data-ttu-id="af1b9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="af1b9-122">Description</span></span>                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="af1b9-123">categories</span><span class="sxs-lookup"><span data-stu-id="af1b9-123">categories</span></span>    |<span data-ttu-id="af1b9-124">String collection</span><span class="sxs-lookup"><span data-stu-id="af1b9-124">String collection</span></span>  | <span data-ttu-id="af1b9-125">Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).</span><span class="sxs-lookup"><span data-stu-id="af1b9-125">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="af1b9-126">description</span><span class="sxs-lookup"><span data-stu-id="af1b9-126">description</span></span>   |<span data-ttu-id="af1b9-127">String</span><span class="sxs-lookup"><span data-stu-id="af1b9-127">String</span></span>             | <span data-ttu-id="af1b9-128">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="af1b9-128">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="af1b9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="af1b9-129">displayName</span></span>   |<span data-ttu-id="af1b9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af1b9-130">String</span></span>             | <span data-ttu-id="af1b9-131">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="af1b9-131">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="af1b9-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="af1b9-132">webUrl</span></span>        |<span data-ttu-id="af1b9-133">String</span><span class="sxs-lookup"><span data-stu-id="af1b9-133">String</span></span>             | <span data-ttu-id="af1b9-134">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="af1b9-134">Contains a link to the website itself.</span></span>                                              |

## <a name="relationships"></a><span data-ttu-id="af1b9-135">Relações</span><span class="sxs-lookup"><span data-stu-id="af1b9-135">Relationships</span></span>

<span data-ttu-id="af1b9-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af1b9-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af1b9-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af1b9-137">JSON representation</span></span>

<span data-ttu-id="af1b9-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af1b9-138">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personWebsite",
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
  "description": "personWebsite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
