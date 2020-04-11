---
title: tipo de recurso personAnniversary
description: tipo de recurso personAnniversary
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c8ea4e9bf7db268c5ec6bffad1c7d43cbbdd2439
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227726"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="038c2-103">tipo de recurso personAnniversary</span><span class="sxs-lookup"><span data-stu-id="038c2-103">personAnniversary resource type</span></span>

<span data-ttu-id="038c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="038c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="038c2-105">Representa os detalhes de datas significativas associadas a uma pessoa em um [perfil](profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="038c2-105">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="038c2-106">Herda de [Myfacet](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="038c2-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="038c2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="038c2-107">Methods</span></span>

| <span data-ttu-id="038c2-108">Método</span><span class="sxs-lookup"><span data-stu-id="038c2-108">Method</span></span>                                                   | <span data-ttu-id="038c2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="038c2-109">Return Type</span></span>                               | <span data-ttu-id="038c2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="038c2-110">Description</span></span>                                                              |
|:---------------------------------------------------------|:------------------------------------------|:-------------------------------------------------------------------------|
| [<span data-ttu-id="038c2-111">Obter personAnniversary</span><span class="sxs-lookup"><span data-stu-id="038c2-111">Get personAnniversary</span></span>](../api/personanniversary-get.md) | [<span data-ttu-id="038c2-112">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="038c2-112">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="038c2-113">Leia as propriedades e os relacionamentos de um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="038c2-113">Read the properties and relationships of a **personAnniversary** object.</span></span> |
| [<span data-ttu-id="038c2-114">Update</span><span class="sxs-lookup"><span data-stu-id="038c2-114">Update</span></span>](../api/personanniversary-update.md)             | [<span data-ttu-id="038c2-115">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="038c2-115">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="038c2-116">Atualizar um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="038c2-116">Update a **personAnniversary** object.</span></span>                                   |
| [<span data-ttu-id="038c2-117">Delete</span><span class="sxs-lookup"><span data-stu-id="038c2-117">Delete</span></span>](../api/personanniversary-delete.md)             | <span data-ttu-id="038c2-118">None</span><span class="sxs-lookup"><span data-stu-id="038c2-118">None</span></span>                                      | <span data-ttu-id="038c2-119">Excluir um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="038c2-119">Delete a **personAnniversary** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="038c2-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="038c2-120">Properties</span></span>

| <span data-ttu-id="038c2-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="038c2-121">Property</span></span>     | <span data-ttu-id="038c2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="038c2-122">Type</span></span>        | <span data-ttu-id="038c2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="038c2-123">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="038c2-124">data</span><span class="sxs-lookup"><span data-stu-id="038c2-124">date</span></span>          |<span data-ttu-id="038c2-125">Data</span><span class="sxs-lookup"><span data-stu-id="038c2-125">Date</span></span>         | <span data-ttu-id="038c2-126">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="038c2-126">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="038c2-127">type</span><span class="sxs-lookup"><span data-stu-id="038c2-127">type</span></span>          |<span data-ttu-id="038c2-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="038c2-128">string</span></span>       | <span data-ttu-id="038c2-129">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="038c2-129">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="038c2-130">Relações</span><span class="sxs-lookup"><span data-stu-id="038c2-130">Relationships</span></span>

<span data-ttu-id="038c2-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="038c2-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="038c2-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="038c2-132">JSON representation</span></span>

<span data-ttu-id="038c2-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="038c2-133">The following is a JSON representation of the resource.</span></span>

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
