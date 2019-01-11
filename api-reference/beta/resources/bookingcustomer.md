---
title: tipo de recurso de bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 02439b16235b3ff1560b5a74b15cd6ce2cb3075b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888974"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="340bc-104">tipo de recurso de bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="340bc-104">bookingCustomer resource type</span></span>

 > <span data-ttu-id="340bc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="340bc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="340bc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="340bc-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="340bc-107">Representa um cliente de um [bookingBsiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="340bc-107">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="340bc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="340bc-108">Methods</span></span>

| <span data-ttu-id="340bc-109">Método</span><span class="sxs-lookup"><span data-stu-id="340bc-109">Method</span></span>           | <span data-ttu-id="340bc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="340bc-110">Return Type</span></span>    |<span data-ttu-id="340bc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="340bc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="340bc-112">Clientes de lista</span><span class="sxs-lookup"><span data-stu-id="340bc-112">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="340bc-113">coleção [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="340bc-113">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="340bc-114">Obtenha uma lista de objetos **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="340bc-114">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="340bc-115">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="340bc-115">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="340bc-116">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="340bc-116">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="340bc-117">Crie um novo objeto de **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="340bc-117">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="340bc-118">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="340bc-118">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="340bc-119">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="340bc-119">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="340bc-120">Leia as propriedades e relacionamentos de um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="340bc-120">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="340bc-121">Update</span><span class="sxs-lookup"><span data-stu-id="340bc-121">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="340bc-122">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="340bc-122">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="340bc-123">Atualize um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="340bc-123">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="340bc-124">Delete</span><span class="sxs-lookup"><span data-stu-id="340bc-124">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="340bc-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="340bc-125">None</span></span> |<span data-ttu-id="340bc-126">Exclua um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="340bc-126">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="340bc-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="340bc-127">Properties</span></span>
| <span data-ttu-id="340bc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="340bc-128">Property</span></span>     | <span data-ttu-id="340bc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="340bc-129">Type</span></span>   |<span data-ttu-id="340bc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="340bc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="340bc-131">displayName</span><span class="sxs-lookup"><span data-stu-id="340bc-131">displayName</span></span>|<span data-ttu-id="340bc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="340bc-132">String</span></span>|<span data-ttu-id="340bc-133">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="340bc-133">The name of the customer.</span></span>|
|<span data-ttu-id="340bc-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="340bc-134">emailAddress</span></span>|<span data-ttu-id="340bc-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="340bc-135">String</span></span>|<span data-ttu-id="340bc-136">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="340bc-136">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="340bc-137">id</span><span class="sxs-lookup"><span data-stu-id="340bc-137">id</span></span>|<span data-ttu-id="340bc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="340bc-138">String</span></span>| <span data-ttu-id="340bc-139">A identificação do cliente.</span><span class="sxs-lookup"><span data-stu-id="340bc-139">The ID of the customer.</span></span> <span data-ttu-id="340bc-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="340bc-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="340bc-141">Relações</span><span class="sxs-lookup"><span data-stu-id="340bc-141">Relationships</span></span>
<span data-ttu-id="340bc-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="340bc-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="340bc-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="340bc-143">JSON representation</span></span>

<span data-ttu-id="340bc-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="340bc-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
