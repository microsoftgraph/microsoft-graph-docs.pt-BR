---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cf4386cf70179715880a1ae07db3dfbb5f07c224
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521894"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="bbbf2-103">tipo de recurso personWebsite</span><span class="sxs-lookup"><span data-stu-id="bbbf2-103">personWebsite resource type</span></span>

<span data-ttu-id="bbbf2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bbbf2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbbf2-105">Representa informações detalhadas sobre sites associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="bbbf2-105">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="bbbf2-106">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="bbbf2-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bbbf2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="bbbf2-107">Methods</span></span>

| <span data-ttu-id="bbbf2-108">Método</span><span class="sxs-lookup"><span data-stu-id="bbbf2-108">Method</span></span>                                           | <span data-ttu-id="bbbf2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bbbf2-109">Return Type</span></span>                       | <span data-ttu-id="bbbf2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbbf2-110">Description</span></span>                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [<span data-ttu-id="bbbf2-111">Obter personWebsite</span><span class="sxs-lookup"><span data-stu-id="bbbf2-111">Get personWebsite</span></span>](../api/personwebsite-get.md) | [<span data-ttu-id="bbbf2-112">personWebsite</span><span class="sxs-lookup"><span data-stu-id="bbbf2-112">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="bbbf2-113">Leia as propriedades e os relacionamentos de um objeto **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="bbbf2-113">Read the properties and relationships of a **personWebsite** object.</span></span> |
| [<span data-ttu-id="bbbf2-114">Atualizar personWebsite</span><span class="sxs-lookup"><span data-stu-id="bbbf2-114">Update personWebsite</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="bbbf2-115">personWebsite</span><span class="sxs-lookup"><span data-stu-id="bbbf2-115">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="bbbf2-116">Atualizar um objeto **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="bbbf2-116">Update a **personWebsite** object.</span></span>                               |
| [<span data-ttu-id="bbbf2-117">Excluir personWebsite</span><span class="sxs-lookup"><span data-stu-id="bbbf2-117">Delete personWebsite</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="bbbf2-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbbf2-118">None</span></span>                              | <span data-ttu-id="bbbf2-119">Excluir um objeto **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="bbbf2-119">Delete a **personWebsite** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="bbbf2-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbbf2-120">Properties</span></span>

| <span data-ttu-id="bbbf2-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbbf2-121">Property</span></span>     | <span data-ttu-id="bbbf2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbbf2-122">Type</span></span>              | <span data-ttu-id="bbbf2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbbf2-123">Description</span></span>                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="bbbf2-124">categories</span><span class="sxs-lookup"><span data-stu-id="bbbf2-124">categories</span></span>    |<span data-ttu-id="bbbf2-125">String collection</span><span class="sxs-lookup"><span data-stu-id="bbbf2-125">String collection</span></span>  | <span data-ttu-id="bbbf2-126">Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).</span><span class="sxs-lookup"><span data-stu-id="bbbf2-126">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="bbbf2-127">description</span><span class="sxs-lookup"><span data-stu-id="bbbf2-127">description</span></span>   |<span data-ttu-id="bbbf2-128">String</span><span class="sxs-lookup"><span data-stu-id="bbbf2-128">String</span></span>             | <span data-ttu-id="bbbf2-129">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="bbbf2-129">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="bbbf2-130">displayName</span><span class="sxs-lookup"><span data-stu-id="bbbf2-130">displayName</span></span>   |<span data-ttu-id="bbbf2-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbbf2-131">String</span></span>             | <span data-ttu-id="bbbf2-132">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="bbbf2-132">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="bbbf2-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="bbbf2-133">webUrl</span></span>        |<span data-ttu-id="bbbf2-134">String</span><span class="sxs-lookup"><span data-stu-id="bbbf2-134">String</span></span>             | <span data-ttu-id="bbbf2-135">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="bbbf2-135">Contains a link to the website itself.</span></span>                                              |

## <a name="relationships"></a><span data-ttu-id="bbbf2-136">Relações</span><span class="sxs-lookup"><span data-stu-id="bbbf2-136">Relationships</span></span>

<span data-ttu-id="bbbf2-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbbf2-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbbf2-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbbf2-138">JSON representation</span></span>

<span data-ttu-id="bbbf2-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbbf2-139">The following is a JSON representation of the resource.</span></span> 

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
