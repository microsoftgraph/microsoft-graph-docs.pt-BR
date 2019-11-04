---
title: tipo de recurso workPosition
description: tipo de recurso workPosition
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2a0d742d289cefac825155a2e8917365c0bb97af
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950462"
---
# <a name="workposition-resource-type"></a><span data-ttu-id="b2002-103">tipo de recurso workPosition</span><span class="sxs-lookup"><span data-stu-id="b2002-103">workPosition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2002-104">Representa informações detalhadas sobre posições de trabalho associadas ao [perfil](profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b2002-104">Represents detailed information about work positions associated with a user's [profile](profile.md).</span></span>

<span data-ttu-id="b2002-105">Esse tipo de recurso herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b2002-105">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b2002-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b2002-106">Methods</span></span>

| <span data-ttu-id="b2002-107">Método</span><span class="sxs-lookup"><span data-stu-id="b2002-107">Method</span></span>                                         | <span data-ttu-id="b2002-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b2002-108">Return Type</span></span>                     | <span data-ttu-id="b2002-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2002-109">Description</span></span>                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [<span data-ttu-id="b2002-110">Obter workPosition</span><span class="sxs-lookup"><span data-stu-id="b2002-110">Get workPosition</span></span>](../api/workposition-get.md) | [<span data-ttu-id="b2002-111">workPosition</span><span class="sxs-lookup"><span data-stu-id="b2002-111">workPosition</span></span>](workposition.md) | <span data-ttu-id="b2002-112">Leia as propriedades e os relacionamentos de um objeto **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="b2002-112">Read the properties and relationships of a **workPosition** object.</span></span> |
| [<span data-ttu-id="b2002-113">Atualizar workPosition</span><span class="sxs-lookup"><span data-stu-id="b2002-113">Update workPosition</span></span>](../api/workposition-update.md)        | [<span data-ttu-id="b2002-114">workPosition</span><span class="sxs-lookup"><span data-stu-id="b2002-114">workPosition</span></span>](workposition.md) | <span data-ttu-id="b2002-115">Atualizar um objeto **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="b2002-115">Update a **workPosition** object.</span></span>                               |
| [<span data-ttu-id="b2002-116">Excluir workPosition</span><span class="sxs-lookup"><span data-stu-id="b2002-116">Delete workPosition</span></span>](../api/workposition-delete.md)        | <span data-ttu-id="b2002-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2002-117">None</span></span>                            | <span data-ttu-id="b2002-118">Excluir um objeto **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="b2002-118">Delete a **workPosition** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="b2002-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2002-119">Properties</span></span>

| <span data-ttu-id="b2002-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2002-120">Property</span></span>             | <span data-ttu-id="b2002-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2002-121">Type</span></span>                               | <span data-ttu-id="b2002-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2002-122">Description</span></span>                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b2002-123">categories</span><span class="sxs-lookup"><span data-stu-id="b2002-123">categories</span></span>            |<span data-ttu-id="b2002-124">String collection</span><span class="sxs-lookup"><span data-stu-id="b2002-124">String collection</span></span>                   | <span data-ttu-id="b2002-125">Contém categorias que um usuário associou à posição (por exemplo, transformação digital, pessoas).</span><span class="sxs-lookup"><span data-stu-id="b2002-125">Contains categories a user has associated with the position (for example, digital transformation, people).</span></span> |
|<span data-ttu-id="b2002-126">detalhada</span><span class="sxs-lookup"><span data-stu-id="b2002-126">detail</span></span>                |[<span data-ttu-id="b2002-127">positionDetail</span><span class="sxs-lookup"><span data-stu-id="b2002-127">positionDetail</span></span>](positiondetail.md) | <span data-ttu-id="b2002-128">Contém detalhes sobre as posições de emprego atuais e anteriores do usuário.</span><span class="sxs-lookup"><span data-stu-id="b2002-128">Contains detail about the user's current and previous employment positions.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="b2002-129">Relações</span><span class="sxs-lookup"><span data-stu-id="b2002-129">Relationships</span></span>

<span data-ttu-id="b2002-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2002-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2002-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2002-131">JSON representation</span></span>

<span data-ttu-id="b2002-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2002-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workPosition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
