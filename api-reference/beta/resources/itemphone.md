---
title: tipo de recurso de Tel.
description: tipo de recurso de Tel.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a40a0a096fa6f0616a8ff44e41e25791873fa82f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939317"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="0b631-103">tipo de recurso de Tel.</span><span class="sxs-lookup"><span data-stu-id="0b631-103">itemPhone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b631-104">Representa informações detalhadas sobre números de telefone que o usuário tenha associado em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="0b631-104">Represents detailed information about phone numbers the user has associated in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="0b631-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b631-105">Methods</span></span>

| <span data-ttu-id="0b631-106">Método</span><span class="sxs-lookup"><span data-stu-id="0b631-106">Method</span></span>                                     | <span data-ttu-id="0b631-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b631-107">Return Type</span></span>               | <span data-ttu-id="0b631-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b631-108">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="0b631-109">Obter o número de telefone</span><span class="sxs-lookup"><span data-stu-id="0b631-109">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="0b631-110">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="0b631-110">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="0b631-111">Leia as propriedades e os relacionamentos de um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="0b631-111">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="0b631-112">Atualizar o número de telefone</span><span class="sxs-lookup"><span data-stu-id="0b631-112">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="0b631-113">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="0b631-113">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="0b631-114">Atualize um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="0b631-114">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="0b631-115">Excluir o número de telefone</span><span class="sxs-lookup"><span data-stu-id="0b631-115">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="0b631-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b631-116">None</span></span>                      | <span data-ttu-id="0b631-117">Excluir um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="0b631-117">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="0b631-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b631-118">Properties</span></span>

| <span data-ttu-id="0b631-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b631-119">Property</span></span>     | <span data-ttu-id="0b631-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b631-120">Type</span></span>        | <span data-ttu-id="0b631-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b631-121">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0b631-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0b631-122">displayName</span></span>   |<span data-ttu-id="0b631-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b631-123">String</span></span>       | <span data-ttu-id="0b631-124">Contém um nome amigável para o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="0b631-124">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="0b631-125">number</span><span class="sxs-lookup"><span data-stu-id="0b631-125">number</span></span>        |<span data-ttu-id="0b631-126">String</span><span class="sxs-lookup"><span data-stu-id="0b631-126">String</span></span>       | <span data-ttu-id="0b631-127">Contém o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="0b631-127">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="0b631-128">type</span><span class="sxs-lookup"><span data-stu-id="0b631-128">type</span></span>          |<span data-ttu-id="0b631-129">string</span><span class="sxs-lookup"><span data-stu-id="0b631-129">string</span></span>       | <span data-ttu-id="0b631-130">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="0b631-130">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b631-131">Relações</span><span class="sxs-lookup"><span data-stu-id="0b631-131">Relationships</span></span>

<span data-ttu-id="0b631-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b631-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b631-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b631-133">JSON representation</span></span>

<span data-ttu-id="0b631-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b631-134">The following is a JSON representation of the resource.</span></span>

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
