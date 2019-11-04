---
title: tipo de recurso de Tel.
description: tipo de recurso de Tel.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2ba1fce4492bfacb3a44f21a0fc55ddd8d37b068
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950434"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="0adf5-103">tipo de recurso de Tel.</span><span class="sxs-lookup"><span data-stu-id="0adf5-103">itemPhone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0adf5-104">Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="0adf5-104">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="0adf5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0adf5-105">Methods</span></span>

| <span data-ttu-id="0adf5-106">Método</span><span class="sxs-lookup"><span data-stu-id="0adf5-106">Method</span></span>                                     | <span data-ttu-id="0adf5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0adf5-107">Return Type</span></span>               | <span data-ttu-id="0adf5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0adf5-108">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="0adf5-109">Obter o número de telefone</span><span class="sxs-lookup"><span data-stu-id="0adf5-109">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="0adf5-110">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="0adf5-110">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="0adf5-111">Leia as propriedades e os relacionamentos de um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="0adf5-111">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="0adf5-112">Atualizar o número de telefone</span><span class="sxs-lookup"><span data-stu-id="0adf5-112">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="0adf5-113">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="0adf5-113">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="0adf5-114">Atualize um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="0adf5-114">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="0adf5-115">Excluir o número de telefone</span><span class="sxs-lookup"><span data-stu-id="0adf5-115">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="0adf5-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0adf5-116">None</span></span>                      | <span data-ttu-id="0adf5-117">Excluir um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="0adf5-117">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="0adf5-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0adf5-118">Properties</span></span>

| <span data-ttu-id="0adf5-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0adf5-119">Property</span></span>     | <span data-ttu-id="0adf5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0adf5-120">Type</span></span>        | <span data-ttu-id="0adf5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0adf5-121">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0adf5-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0adf5-122">displayName</span></span>   |<span data-ttu-id="0adf5-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0adf5-123">String</span></span>       | <span data-ttu-id="0adf5-124">Contém um nome amigável para o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="0adf5-124">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="0adf5-125">number</span><span class="sxs-lookup"><span data-stu-id="0adf5-125">number</span></span>        |<span data-ttu-id="0adf5-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0adf5-126">String</span></span>       | <span data-ttu-id="0adf5-127">Contém o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="0adf5-127">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="0adf5-128">type</span><span class="sxs-lookup"><span data-stu-id="0adf5-128">type</span></span>          |<span data-ttu-id="0adf5-129">string</span><span class="sxs-lookup"><span data-stu-id="0adf5-129">string</span></span>       | <span data-ttu-id="0adf5-130">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="0adf5-130">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0adf5-131">Relações</span><span class="sxs-lookup"><span data-stu-id="0adf5-131">Relationships</span></span>

<span data-ttu-id="0adf5-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0adf5-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0adf5-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0adf5-133">JSON representation</span></span>

<span data-ttu-id="0adf5-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0adf5-134">The following is a JSON representation of the resource.</span></span>

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
