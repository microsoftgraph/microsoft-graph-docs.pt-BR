---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0be7c3863f9c764e7b6a0c0a4d0d8b2e9dc30717
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939590"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="1ebd8-103">tipo de recurso personWebsite</span><span class="sxs-lookup"><span data-stu-id="1ebd8-103">personWebsite resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ebd8-104">Representa informações detalhadas sobre sites que o usuário tenha associado a si mesmos em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-104">Represents detailed information about websites the user has associated with themselves in various services.</span></span>

<span data-ttu-id="1ebd8-105">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1ebd8-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1ebd8-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1ebd8-106">Methods</span></span>

| <span data-ttu-id="1ebd8-107">Método</span><span class="sxs-lookup"><span data-stu-id="1ebd8-107">Method</span></span>                                           | <span data-ttu-id="1ebd8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1ebd8-108">Return Type</span></span>                       | <span data-ttu-id="1ebd8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ebd8-109">Description</span></span>                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [<span data-ttu-id="1ebd8-110">Obter personWebsite</span><span class="sxs-lookup"><span data-stu-id="1ebd8-110">Get personWebsite</span></span>](../api/personwebsite-get.md) | [<span data-ttu-id="1ebd8-111">personWebsite</span><span class="sxs-lookup"><span data-stu-id="1ebd8-111">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="1ebd8-112">Leia as propriedades e os relacionamentos do objeto personWebsite.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-112">Read properties and relationships of personWebsite object.</span></span> |
| [<span data-ttu-id="1ebd8-113">Update</span><span class="sxs-lookup"><span data-stu-id="1ebd8-113">Update</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="1ebd8-114">personWebsite</span><span class="sxs-lookup"><span data-stu-id="1ebd8-114">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="1ebd8-115">Atualize o objeto personWebsite.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-115">Update personWebsite object.</span></span>                               |
| [<span data-ttu-id="1ebd8-116">Delete</span><span class="sxs-lookup"><span data-stu-id="1ebd8-116">Delete</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="1ebd8-117">None</span><span class="sxs-lookup"><span data-stu-id="1ebd8-117">None</span></span>                              | <span data-ttu-id="1ebd8-118">Exclua o objeto personWebsite.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-118">Delete personWebsite object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="1ebd8-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ebd8-119">Properties</span></span>

| <span data-ttu-id="1ebd8-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ebd8-120">Property</span></span>     | <span data-ttu-id="1ebd8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ebd8-121">Type</span></span>              | <span data-ttu-id="1ebd8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ebd8-122">Description</span></span>                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="1ebd8-123">categories</span><span class="sxs-lookup"><span data-stu-id="1ebd8-123">categories</span></span>    |<span data-ttu-id="1ebd8-124">String collection</span><span class="sxs-lookup"><span data-stu-id="1ebd8-124">String collection</span></span>  | <span data-ttu-id="1ebd8-125">Contém categorias que um usuário associou ao site (por exemplo: pessoal, receitas)</span><span class="sxs-lookup"><span data-stu-id="1ebd8-125">Contains categories a user has associated with the website (eg: personal, recipes)</span></span>  |
|<span data-ttu-id="1ebd8-126">description</span><span class="sxs-lookup"><span data-stu-id="1ebd8-126">description</span></span>   |<span data-ttu-id="1ebd8-127">String</span><span class="sxs-lookup"><span data-stu-id="1ebd8-127">String</span></span>             | <span data-ttu-id="1ebd8-128">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-128">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="1ebd8-129">displayName</span><span class="sxs-lookup"><span data-stu-id="1ebd8-129">displayName</span></span>   |<span data-ttu-id="1ebd8-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ebd8-130">String</span></span>             | <span data-ttu-id="1ebd8-131">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-131">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="1ebd8-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="1ebd8-132">webUrl</span></span>        |<span data-ttu-id="1ebd8-133">String</span><span class="sxs-lookup"><span data-stu-id="1ebd8-133">String</span></span>             | <span data-ttu-id="1ebd8-134">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-134">Contains a link to the website itself.</span></span>                                              |

## <a name="relationships"></a><span data-ttu-id="1ebd8-135">Relações</span><span class="sxs-lookup"><span data-stu-id="1ebd8-135">Relationships</span></span>

<span data-ttu-id="1ebd8-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ebd8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ebd8-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ebd8-137">JSON representation</span></span>

<span data-ttu-id="1ebd8-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ebd8-138">The following is a JSON representation of the resource.</span></span> 

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