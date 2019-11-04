---
title: tipo de recurso personAnniversary
description: tipo de recurso personAnniversary
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1ad4c5a1792ee0e75a31f165b0a8eebf6f0d2130
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949514"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="f7b07-103">tipo de recurso personAnniversary</span><span class="sxs-lookup"><span data-stu-id="f7b07-103">personAnniversary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b07-104">Representa os detalhes de datas significativas associadas a uma pessoa em um [perfil](profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="f7b07-104">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="f7b07-105">Herda de [Myfacet](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="f7b07-105">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f7b07-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f7b07-106">Methods</span></span>

| <span data-ttu-id="f7b07-107">Método</span><span class="sxs-lookup"><span data-stu-id="f7b07-107">Method</span></span>                                                   | <span data-ttu-id="f7b07-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f7b07-108">Return Type</span></span>                               | <span data-ttu-id="f7b07-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7b07-109">Description</span></span>                                                    |
|:---------------------------------------------------------|:------------------------------------------|:---------------------------------------------------------------|
| [<span data-ttu-id="f7b07-110">Obter personAnniversary</span><span class="sxs-lookup"><span data-stu-id="f7b07-110">Get personAnniversary</span></span>](../api/personanniversary-get.md) | [<span data-ttu-id="f7b07-111">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="f7b07-111">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="f7b07-112">Leia as propriedades e os relacionamentos de um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="f7b07-112">Read the properties and relationships of a **personAnniversary** object.</span></span> |
| [<span data-ttu-id="f7b07-113">Update</span><span class="sxs-lookup"><span data-stu-id="f7b07-113">Update</span></span>](../api/personanniversary-update.md)             | [<span data-ttu-id="f7b07-114">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="f7b07-114">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="f7b07-115">Atualizar um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="f7b07-115">Update a **personAnniversary** object.</span></span>                               |
| [<span data-ttu-id="f7b07-116">Delete</span><span class="sxs-lookup"><span data-stu-id="f7b07-116">Delete</span></span>](../api/personanniversary-delete.md)             | <span data-ttu-id="f7b07-117">None</span><span class="sxs-lookup"><span data-stu-id="f7b07-117">None</span></span>                                      | <span data-ttu-id="f7b07-118">Excluir um objeto **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="f7b07-118">Delete a **personAnniversary** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="f7b07-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7b07-119">Properties</span></span>

| <span data-ttu-id="f7b07-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7b07-120">Property</span></span>     | <span data-ttu-id="f7b07-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7b07-121">Type</span></span>        | <span data-ttu-id="f7b07-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7b07-122">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="f7b07-123">data</span><span class="sxs-lookup"><span data-stu-id="f7b07-123">date</span></span>          |<span data-ttu-id="f7b07-124">Data</span><span class="sxs-lookup"><span data-stu-id="f7b07-124">Date</span></span>         | <span data-ttu-id="f7b07-125">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="f7b07-125">Contains the date associated with the anniversary type.</span></span>         |
|<span data-ttu-id="f7b07-126">type</span><span class="sxs-lookup"><span data-stu-id="f7b07-126">type</span></span>          |<span data-ttu-id="f7b07-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7b07-127">string</span></span>       | <span data-ttu-id="f7b07-128">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f7b07-128">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7b07-129">Relações</span><span class="sxs-lookup"><span data-stu-id="f7b07-129">Relationships</span></span>

<span data-ttu-id="f7b07-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7b07-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7b07-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7b07-131">JSON representation</span></span>

<span data-ttu-id="f7b07-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7b07-132">The following is a JSON representation of the resource.</span></span> 

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
