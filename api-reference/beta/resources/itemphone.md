---
title: tipo de recurso de Tel.
description: tipo de recurso de Tel.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 48c585a05043b4f17e5e7406eb44b9150b5e5bdc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523062"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="5e679-103">tipo de recurso de Tel.</span><span class="sxs-lookup"><span data-stu-id="5e679-103">itemPhone resource type</span></span>

<span data-ttu-id="5e679-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5e679-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e679-105">Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="5e679-105">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="5e679-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e679-106">Methods</span></span>

| <span data-ttu-id="5e679-107">Método</span><span class="sxs-lookup"><span data-stu-id="5e679-107">Method</span></span>                                     | <span data-ttu-id="5e679-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e679-108">Return Type</span></span>               | <span data-ttu-id="5e679-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e679-109">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="5e679-110">Obter o número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e679-110">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="5e679-111">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e679-111">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="5e679-112">Leia as propriedades e os relacionamentos de um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="5e679-112">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="5e679-113">Atualizar o número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e679-113">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="5e679-114">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e679-114">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="5e679-115">Atualize um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="5e679-115">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="5e679-116">Excluir o número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e679-116">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="5e679-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e679-117">None</span></span>                      | <span data-ttu-id="5e679-118">Excluir um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="5e679-118">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="5e679-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e679-119">Properties</span></span>

| <span data-ttu-id="5e679-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e679-120">Property</span></span>     | <span data-ttu-id="5e679-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e679-121">Type</span></span>        | <span data-ttu-id="5e679-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e679-122">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5e679-123">displayName</span><span class="sxs-lookup"><span data-stu-id="5e679-123">displayName</span></span>   |<span data-ttu-id="5e679-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e679-124">String</span></span>       | <span data-ttu-id="5e679-125">Contém um nome amigável para o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="5e679-125">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="5e679-126">number</span><span class="sxs-lookup"><span data-stu-id="5e679-126">number</span></span>        |<span data-ttu-id="5e679-127">String</span><span class="sxs-lookup"><span data-stu-id="5e679-127">String</span></span>       | <span data-ttu-id="5e679-128">Contém o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="5e679-128">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="5e679-129">type</span><span class="sxs-lookup"><span data-stu-id="5e679-129">type</span></span>          |<span data-ttu-id="5e679-130">string</span><span class="sxs-lookup"><span data-stu-id="5e679-130">string</span></span>       | <span data-ttu-id="5e679-131">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="5e679-131">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e679-132">Relações</span><span class="sxs-lookup"><span data-stu-id="5e679-132">Relationships</span></span>

<span data-ttu-id="5e679-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e679-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e679-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e679-134">JSON representation</span></span>

<span data-ttu-id="5e679-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e679-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "number": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemPhone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
