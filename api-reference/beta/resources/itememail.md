---
title: tipo de recurso de email
description: tipo de recurso de email
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: eed73f61b281463848c8520ebdcdbc75ac26d29d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939331"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="56bff-103">tipo de recurso de email</span><span class="sxs-lookup"><span data-stu-id="56bff-103">itemEmail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56bff-104">Representa informações detalhadas sobre endereços de email associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="56bff-104">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="56bff-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="56bff-105">Methods</span></span>

| <span data-ttu-id="56bff-106">Método</span><span class="sxs-lookup"><span data-stu-id="56bff-106">Method</span></span>                                   | <span data-ttu-id="56bff-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56bff-107">Return Type</span></span>               | <span data-ttu-id="56bff-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="56bff-108">Description</span></span>                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="56bff-109">Get</span><span class="sxs-lookup"><span data-stu-id="56bff-109">Get</span></span>](../api/itememail-get.md) | [<span data-ttu-id="56bff-110">Email</span><span class="sxs-lookup"><span data-stu-id="56bff-110">itemEmail</span></span>](itememail.md) | <span data-ttu-id="56bff-111">Ler propriedades e relações de um objeto item de **email** .</span><span class="sxs-lookup"><span data-stu-id="56bff-111">Read properties and relationships of an **itemEmail** object.</span></span> |
| [<span data-ttu-id="56bff-112">Update</span><span class="sxs-lookup"><span data-stu-id="56bff-112">Update</span></span>](../api/itememail-update.md)     | [<span data-ttu-id="56bff-113">Email</span><span class="sxs-lookup"><span data-stu-id="56bff-113">itemEmail</span></span>](itememail.md) | <span data-ttu-id="56bff-114">Atualize um objeto de **email** .</span><span class="sxs-lookup"><span data-stu-id="56bff-114">Update an **itemEmail** object.</span></span>                               |
| [<span data-ttu-id="56bff-115">Delete</span><span class="sxs-lookup"><span data-stu-id="56bff-115">Delete</span></span>](../api/itememail-delete.md)     | <span data-ttu-id="56bff-116">None</span><span class="sxs-lookup"><span data-stu-id="56bff-116">None</span></span>                      | <span data-ttu-id="56bff-117">Excluir um objeto de **email** .</span><span class="sxs-lookup"><span data-stu-id="56bff-117">Delete an **itemEmail** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="56bff-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56bff-118">Properties</span></span>

| <span data-ttu-id="56bff-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56bff-119">Property</span></span>     | <span data-ttu-id="56bff-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="56bff-120">Type</span></span>        | <span data-ttu-id="56bff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="56bff-121">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="56bff-122">address</span><span class="sxs-lookup"><span data-stu-id="56bff-122">address</span></span>       |<span data-ttu-id="56bff-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56bff-123">String</span></span>       | <span data-ttu-id="56bff-124">O próprio endereço de email.</span><span class="sxs-lookup"><span data-stu-id="56bff-124">The email address itself.</span></span>                                                 |
|<span data-ttu-id="56bff-125">displayName</span><span class="sxs-lookup"><span data-stu-id="56bff-125">displayName</span></span>   |<span data-ttu-id="56bff-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56bff-126">String</span></span>       | <span data-ttu-id="56bff-127">O nome ou rótulo que um usuário associou a um endereço de email específico.</span><span class="sxs-lookup"><span data-stu-id="56bff-127">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="56bff-128">type</span><span class="sxs-lookup"><span data-stu-id="56bff-128">type</span></span>          |<span data-ttu-id="56bff-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56bff-129">string</span></span>       | <span data-ttu-id="56bff-130">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="56bff-130">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="56bff-131">Relações</span><span class="sxs-lookup"><span data-stu-id="56bff-131">Relationships</span></span>

<span data-ttu-id="56bff-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56bff-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56bff-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56bff-133">JSON representation</span></span>

<span data-ttu-id="56bff-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56bff-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": ""
}-->

```json
{
  "address": "String",
  "displayName": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemEmail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
