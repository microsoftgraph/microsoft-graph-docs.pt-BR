---
title: tipo de recurso personAnniversary
description: tipo de recurso personAnniversary
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7dad5536eb78b2d7119ace63eb0f7ce16880e85f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521922"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="d5708-103">tipo de recurso personAnniversary</span><span class="sxs-lookup"><span data-stu-id="d5708-103">personAnniversary resource type</span></span>

<span data-ttu-id="d5708-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d5708-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5708-105">Representa os detalhes de datas significativas associadas a uma pessoa em um [perfil](profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="d5708-105">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="d5708-106">Herda de [Myfacet](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="d5708-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d5708-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5708-107">Methods</span></span>

| <span data-ttu-id="d5708-108">Método</span><span class="sxs-lookup"><span data-stu-id="d5708-108">Method</span></span>                                                   | <span data-ttu-id="d5708-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5708-109">Return Type</span></span>                               | <span data-ttu-id="d5708-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5708-110">Description</span></span>                                                    |
|:---------------------------------------------------------|:------------------------------------------|:---------------------------------------------------------------|
| [<span data-ttu-id="d5708-111">Obter personAnniversary</span><span class="sxs-lookup"><span data-stu-id="d5708-111">Get personAnniversary</span></span>](../api/personanniversary-get.md) | [<span data-ttu-id="d5708-112">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="d5708-112">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="d5708-113">Leia as propriedades e os relacionamentos de um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="d5708-113">Read the properties and relationships of a **personAnniversary** object.</span></span> |
| [<span data-ttu-id="d5708-114">Update</span><span class="sxs-lookup"><span data-stu-id="d5708-114">Update</span></span>](../api/personanniversary-update.md)             | [<span data-ttu-id="d5708-115">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="d5708-115">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="d5708-116">Atualizar um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="d5708-116">Update a **personAnniversary** object.</span></span>                               |
| [<span data-ttu-id="d5708-117">Delete</span><span class="sxs-lookup"><span data-stu-id="d5708-117">Delete</span></span>](../api/personanniversary-delete.md)             | <span data-ttu-id="d5708-118">None</span><span class="sxs-lookup"><span data-stu-id="d5708-118">None</span></span>                                      | <span data-ttu-id="d5708-119">Excluir um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="d5708-119">Delete a **personAnniversary** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="d5708-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5708-120">Properties</span></span>

| <span data-ttu-id="d5708-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5708-121">Property</span></span>     | <span data-ttu-id="d5708-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5708-122">Type</span></span>        | <span data-ttu-id="d5708-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5708-123">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="d5708-124">data</span><span class="sxs-lookup"><span data-stu-id="d5708-124">date</span></span>          |<span data-ttu-id="d5708-125">Data</span><span class="sxs-lookup"><span data-stu-id="d5708-125">Date</span></span>         | <span data-ttu-id="d5708-126">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="d5708-126">Contains the date associated with the anniversary type.</span></span>         |
|<span data-ttu-id="d5708-127">type</span><span class="sxs-lookup"><span data-stu-id="d5708-127">type</span></span>          |<span data-ttu-id="d5708-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5708-128">string</span></span>       | <span data-ttu-id="d5708-129">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d5708-129">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5708-130">Relações</span><span class="sxs-lookup"><span data-stu-id="d5708-130">Relationships</span></span>

<span data-ttu-id="d5708-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5708-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5708-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5708-132">JSON representation</span></span>

<span data-ttu-id="d5708-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5708-133">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": ""
}-->

```json
{
  "date": "String (timestamp)",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personAnniversary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
