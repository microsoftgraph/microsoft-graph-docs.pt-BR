---
title: tipo de recurso personInterest
description: tipo de recurso personInterest
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1da3ad429011da62f49105c6f352c86ec0741cd4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521908"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="e9d82-103">tipo de recurso personInterest</span><span class="sxs-lookup"><span data-stu-id="e9d82-103">personInterest resource type</span></span>

<span data-ttu-id="e9d82-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e9d82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9d82-105">Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="e9d82-105">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="e9d82-106">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e9d82-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e9d82-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e9d82-107">Methods</span></span>

| <span data-ttu-id="e9d82-108">Método</span><span class="sxs-lookup"><span data-stu-id="e9d82-108">Method</span></span>       | <span data-ttu-id="e9d82-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e9d82-109">Return Type</span></span> | <span data-ttu-id="e9d82-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9d82-110">Description</span></span> |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [<span data-ttu-id="e9d82-111">Obter personInterest</span><span class="sxs-lookup"><span data-stu-id="e9d82-111">Get personInterest</span></span>](../api/personinterest-get.md) | [<span data-ttu-id="e9d82-112">personInterest</span><span class="sxs-lookup"><span data-stu-id="e9d82-112">personInterest</span></span>](personinterest.md) | <span data-ttu-id="e9d82-113">Leia as propriedades e os relacionamentos de um objeto **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="e9d82-113">Read the properties and relationships of a **personInterest** object.</span></span> |
| [<span data-ttu-id="e9d82-114">Atualizar personInterest</span><span class="sxs-lookup"><span data-stu-id="e9d82-114">Update personInterest</span></span>](../api/personinterest-update.md)          | [<span data-ttu-id="e9d82-115">personInterest</span><span class="sxs-lookup"><span data-stu-id="e9d82-115">personInterest</span></span>](personinterest.md) | <span data-ttu-id="e9d82-116">Atualizar um objeto **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="e9d82-116">Update a **personInterest** object.</span></span>                               |
| [<span data-ttu-id="e9d82-117">Excluir personInterest</span><span class="sxs-lookup"><span data-stu-id="e9d82-117">Delete personInterest</span></span>](../api/personinterest-delete.md)          | <span data-ttu-id="e9d82-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9d82-118">None</span></span>                                | <span data-ttu-id="e9d82-119">Excluir um objeto **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="e9d82-119">Delete a **personInterest** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="e9d82-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9d82-120">Properties</span></span>

| <span data-ttu-id="e9d82-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9d82-121">Property</span></span>     | <span data-ttu-id="e9d82-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9d82-122">Type</span></span>             | <span data-ttu-id="e9d82-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9d82-123">Description</span></span>                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|<span data-ttu-id="e9d82-124">categories</span><span class="sxs-lookup"><span data-stu-id="e9d82-124">categories</span></span>    |<span data-ttu-id="e9d82-125">String collection</span><span class="sxs-lookup"><span data-stu-id="e9d82-125">String collection</span></span> | <span data-ttu-id="e9d82-126">Contém categorias que um usuário associou aos juros (por exemplo, pessoal, recipies).</span><span class="sxs-lookup"><span data-stu-id="e9d82-126">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="e9d82-127">description</span><span class="sxs-lookup"><span data-stu-id="e9d82-127">description</span></span>   |<span data-ttu-id="e9d82-128">String</span><span class="sxs-lookup"><span data-stu-id="e9d82-128">String</span></span>            | <span data-ttu-id="e9d82-129">Contém uma descrição dos juros.</span><span class="sxs-lookup"><span data-stu-id="e9d82-129">Contains a description of the interest.</span></span>                                              |
|<span data-ttu-id="e9d82-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e9d82-130">displayName</span></span>   |<span data-ttu-id="e9d82-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9d82-131">String</span></span>            | <span data-ttu-id="e9d82-132">Contém um nome amigável para os juros.</span><span class="sxs-lookup"><span data-stu-id="e9d82-132">Contains a friendly name for the interest.</span></span>                                           |
|<span data-ttu-id="e9d82-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="e9d82-133">webUrl</span></span>        |<span data-ttu-id="e9d82-134">String</span><span class="sxs-lookup"><span data-stu-id="e9d82-134">String</span></span>            | <span data-ttu-id="e9d82-135">Contém um link para uma página da Web ou recurso sobre os juros.</span><span class="sxs-lookup"><span data-stu-id="e9d82-135">Contains a link to a web page or resource about the interest.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="e9d82-136">Relações</span><span class="sxs-lookup"><span data-stu-id="e9d82-136">Relationships</span></span>

<span data-ttu-id="e9d82-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9d82-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9d82-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9d82-138">JSON representation</span></span>

<span data-ttu-id="e9d82-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9d82-139">The following is a JSON representation of the resource.</span></span> 

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
