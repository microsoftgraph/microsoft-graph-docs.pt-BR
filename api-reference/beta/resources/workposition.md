---
title: tipo de recurso workPosition
description: tipo de recurso workPosition
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 086273e54d923054ce8e71ef1c67fb2bb4f7002a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519061"
---
# <a name="workposition-resource-type"></a><span data-ttu-id="76a59-103">tipo de recurso workPosition</span><span class="sxs-lookup"><span data-stu-id="76a59-103">workPosition resource type</span></span>

<span data-ttu-id="76a59-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="76a59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76a59-105">Representa informações detalhadas sobre posições de trabalho associadas ao [perfil](profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="76a59-105">Represents detailed information about work positions associated with a user's [profile](profile.md).</span></span>

<span data-ttu-id="76a59-106">Esse tipo de recurso herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76a59-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="76a59-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="76a59-107">Methods</span></span>

| <span data-ttu-id="76a59-108">Método</span><span class="sxs-lookup"><span data-stu-id="76a59-108">Method</span></span>                                         | <span data-ttu-id="76a59-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="76a59-109">Return Type</span></span>                     | <span data-ttu-id="76a59-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="76a59-110">Description</span></span>                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [<span data-ttu-id="76a59-111">Obter workPosition</span><span class="sxs-lookup"><span data-stu-id="76a59-111">Get workPosition</span></span>](../api/workposition-get.md) | [<span data-ttu-id="76a59-112">workPosition</span><span class="sxs-lookup"><span data-stu-id="76a59-112">workPosition</span></span>](workposition.md) | <span data-ttu-id="76a59-113">Leia as propriedades e os relacionamentos de um objeto **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="76a59-113">Read the properties and relationships of a **workPosition** object.</span></span> |
| [<span data-ttu-id="76a59-114">Atualizar workPosition</span><span class="sxs-lookup"><span data-stu-id="76a59-114">Update workPosition</span></span>](../api/workposition-update.md)        | [<span data-ttu-id="76a59-115">workPosition</span><span class="sxs-lookup"><span data-stu-id="76a59-115">workPosition</span></span>](workposition.md) | <span data-ttu-id="76a59-116">Atualizar um objeto **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="76a59-116">Update a **workPosition** object.</span></span>                               |
| [<span data-ttu-id="76a59-117">Excluir workPosition</span><span class="sxs-lookup"><span data-stu-id="76a59-117">Delete workPosition</span></span>](../api/workposition-delete.md)        | <span data-ttu-id="76a59-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76a59-118">None</span></span>                            | <span data-ttu-id="76a59-119">Excluir um objeto **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="76a59-119">Delete a **workPosition** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="76a59-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76a59-120">Properties</span></span>

| <span data-ttu-id="76a59-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76a59-121">Property</span></span>             | <span data-ttu-id="76a59-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="76a59-122">Type</span></span>                               | <span data-ttu-id="76a59-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="76a59-123">Description</span></span>                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="76a59-124">categories</span><span class="sxs-lookup"><span data-stu-id="76a59-124">categories</span></span>            |<span data-ttu-id="76a59-125">String collection</span><span class="sxs-lookup"><span data-stu-id="76a59-125">String collection</span></span>                   | <span data-ttu-id="76a59-126">Contém categorias que um usuário associou à posição (por exemplo, transformação digital, pessoas).</span><span class="sxs-lookup"><span data-stu-id="76a59-126">Contains categories a user has associated with the position (for example, digital transformation, people).</span></span> |
|<span data-ttu-id="76a59-127">detalhada</span><span class="sxs-lookup"><span data-stu-id="76a59-127">detail</span></span>                |[<span data-ttu-id="76a59-128">positionDetail</span><span class="sxs-lookup"><span data-stu-id="76a59-128">positionDetail</span></span>](positiondetail.md) | <span data-ttu-id="76a59-129">Contém detalhes sobre as posições de emprego atuais e anteriores do usuário.</span><span class="sxs-lookup"><span data-stu-id="76a59-129">Contains detail about the user's current and previous employment positions.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="76a59-130">Relações</span><span class="sxs-lookup"><span data-stu-id="76a59-130">Relationships</span></span>

<span data-ttu-id="76a59-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76a59-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76a59-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76a59-132">JSON representation</span></span>

<span data-ttu-id="76a59-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76a59-133">The following is a JSON representation of the resource.</span></span>

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
