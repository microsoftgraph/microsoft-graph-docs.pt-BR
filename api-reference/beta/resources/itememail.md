---
title: tipo de recurso de email
description: tipo de recurso de email
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aaf58bd7e20caeb418946814daa7ca8f7bb9bfa3
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229413"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="a2843-103">tipo de recurso de email</span><span class="sxs-lookup"><span data-stu-id="a2843-103">itemEmail resource type</span></span>

<span data-ttu-id="a2843-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2843-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2843-105">Representa informações detalhadas sobre endereços de email associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a2843-105">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="a2843-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2843-106">Methods</span></span>

| <span data-ttu-id="a2843-107">Método</span><span class="sxs-lookup"><span data-stu-id="a2843-107">Method</span></span>                                   | <span data-ttu-id="a2843-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2843-108">Return Type</span></span>               | <span data-ttu-id="a2843-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2843-109">Description</span></span>                                                      |
|:-----------------------------------------|:--------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="a2843-110">Get</span><span class="sxs-lookup"><span data-stu-id="a2843-110">Get</span></span>](../api/itememail-get.md)           | [<span data-ttu-id="a2843-111">Email</span><span class="sxs-lookup"><span data-stu-id="a2843-111">itemEmail</span></span>](itememail.md) | <span data-ttu-id="a2843-112">Ler propriedades e relações de um objeto item de **email** .</span><span class="sxs-lookup"><span data-stu-id="a2843-112">Read properties and relationships of an **itemEmail** object.</span></span>    |
| [<span data-ttu-id="a2843-113">Update</span><span class="sxs-lookup"><span data-stu-id="a2843-113">Update</span></span>](../api/itememail-update.md)     | [<span data-ttu-id="a2843-114">Email</span><span class="sxs-lookup"><span data-stu-id="a2843-114">itemEmail</span></span>](itememail.md) | <span data-ttu-id="a2843-115">Atualize um objeto de **email** .</span><span class="sxs-lookup"><span data-stu-id="a2843-115">Update an **itemEmail** object.</span></span>                                  |
| [<span data-ttu-id="a2843-116">Delete</span><span class="sxs-lookup"><span data-stu-id="a2843-116">Delete</span></span>](../api/itememail-delete.md)     | <span data-ttu-id="a2843-117">None</span><span class="sxs-lookup"><span data-stu-id="a2843-117">None</span></span>                      | <span data-ttu-id="a2843-118">Excluir um objeto de **email** .</span><span class="sxs-lookup"><span data-stu-id="a2843-118">Delete an **itemEmail** object.</span></span>                                  |

## <a name="properties"></a><span data-ttu-id="a2843-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2843-119">Properties</span></span>

| <span data-ttu-id="a2843-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2843-120">Property</span></span>     | <span data-ttu-id="a2843-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2843-121">Type</span></span>        | <span data-ttu-id="a2843-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2843-122">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="a2843-123">address</span><span class="sxs-lookup"><span data-stu-id="a2843-123">address</span></span>       |<span data-ttu-id="a2843-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2843-124">String</span></span>       | <span data-ttu-id="a2843-125">O próprio endereço de email.</span><span class="sxs-lookup"><span data-stu-id="a2843-125">The email address itself.</span></span>                                                 |
|<span data-ttu-id="a2843-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a2843-126">displayName</span></span>   |<span data-ttu-id="a2843-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2843-127">String</span></span>       | <span data-ttu-id="a2843-128">O nome ou rótulo que um usuário associou a um endereço de email específico.</span><span class="sxs-lookup"><span data-stu-id="a2843-128">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="a2843-129">type</span><span class="sxs-lookup"><span data-stu-id="a2843-129">type</span></span>          |<span data-ttu-id="a2843-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2843-130">string</span></span>       | <span data-ttu-id="a2843-131">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="a2843-131">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="a2843-132">Relações</span><span class="sxs-lookup"><span data-stu-id="a2843-132">Relationships</span></span>

<span data-ttu-id="a2843-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2843-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2843-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2843-134">JSON representation</span></span>

<span data-ttu-id="a2843-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2843-135">The following is a JSON representation of the resource.</span></span>

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
