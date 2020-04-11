---
title: tipo de recurso de Tel.
description: tipo de recurso de Tel.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4bc101ca8cbfb063fa1bba3a2ebdb4e6afc2fd57
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229399"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="cd6ad-103">tipo de recurso de Tel.</span><span class="sxs-lookup"><span data-stu-id="cd6ad-103">itemPhone resource type</span></span>

<span data-ttu-id="cd6ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd6ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd6ad-105">Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="cd6ad-105">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="cd6ad-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd6ad-106">Methods</span></span>

| <span data-ttu-id="cd6ad-107">Método</span><span class="sxs-lookup"><span data-stu-id="cd6ad-107">Method</span></span>                                               | <span data-ttu-id="cd6ad-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd6ad-108">Return Type</span></span>               | <span data-ttu-id="cd6ad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd6ad-109">Description</span></span>                                                       |
|:-----------------------------------------------------|:--------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="cd6ad-110">Obter o número de telefone</span><span class="sxs-lookup"><span data-stu-id="cd6ad-110">Get itemPhone</span></span>](../api/itemphone-get.md)             | [<span data-ttu-id="cd6ad-111">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="cd6ad-111">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="cd6ad-112">Leia as propriedades e os relacionamentos de um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="cd6ad-112">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="cd6ad-113">Atualizar o número de telefone</span><span class="sxs-lookup"><span data-stu-id="cd6ad-113">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="cd6ad-114">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="cd6ad-114">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="cd6ad-115">Atualize um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="cd6ad-115">Update an **itemPhone** object.</span></span>                                   |
| [<span data-ttu-id="cd6ad-116">Excluir o número de telefone</span><span class="sxs-lookup"><span data-stu-id="cd6ad-116">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="cd6ad-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd6ad-117">None</span></span>                      | <span data-ttu-id="cd6ad-118">Excluir um objeto **MyPhone** .</span><span class="sxs-lookup"><span data-stu-id="cd6ad-118">Delete an **itemPhone** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="cd6ad-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd6ad-119">Properties</span></span>

| <span data-ttu-id="cd6ad-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd6ad-120">Property</span></span>     | <span data-ttu-id="cd6ad-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd6ad-121">Type</span></span>        | <span data-ttu-id="cd6ad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd6ad-122">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="cd6ad-123">displayName</span><span class="sxs-lookup"><span data-stu-id="cd6ad-123">displayName</span></span>   |<span data-ttu-id="cd6ad-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd6ad-124">String</span></span>       | <span data-ttu-id="cd6ad-125">Contém um nome amigável para o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="cd6ad-125">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="cd6ad-126">number</span><span class="sxs-lookup"><span data-stu-id="cd6ad-126">number</span></span>        |<span data-ttu-id="cd6ad-127">String</span><span class="sxs-lookup"><span data-stu-id="cd6ad-127">String</span></span>       | <span data-ttu-id="cd6ad-128">Contém o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="cd6ad-128">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="cd6ad-129">type</span><span class="sxs-lookup"><span data-stu-id="cd6ad-129">type</span></span>          |<span data-ttu-id="cd6ad-130">string</span><span class="sxs-lookup"><span data-stu-id="cd6ad-130">string</span></span>       | <span data-ttu-id="cd6ad-131">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="cd6ad-131">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd6ad-132">Relações</span><span class="sxs-lookup"><span data-stu-id="cd6ad-132">Relationships</span></span>

<span data-ttu-id="cd6ad-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd6ad-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd6ad-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd6ad-134">JSON representation</span></span>

<span data-ttu-id="cd6ad-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd6ad-135">The following is a JSON representation of the resource.</span></span>

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
