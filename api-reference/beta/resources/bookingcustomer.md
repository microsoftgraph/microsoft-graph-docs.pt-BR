---
title: tipo de recurso bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5b527902c5d6e39bb752e07838c6a5e1c3022bb0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071784"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="56dd1-104">tipo de recurso bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="56dd1-104">bookingCustomer resource type</span></span>

<span data-ttu-id="56dd1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56dd1-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="56dd1-106">Representa um cliente de um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="56dd1-106">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="56dd1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="56dd1-107">Methods</span></span>

| <span data-ttu-id="56dd1-108">Método</span><span class="sxs-lookup"><span data-stu-id="56dd1-108">Method</span></span>           | <span data-ttu-id="56dd1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56dd1-109">Return Type</span></span>    |<span data-ttu-id="56dd1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="56dd1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56dd1-111">Listar clientes</span><span class="sxs-lookup"><span data-stu-id="56dd1-111">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="56dd1-112">coleção [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="56dd1-112">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="56dd1-113">Obtenha uma lista de objetos **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="56dd1-113">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="56dd1-114">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="56dd1-114">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="56dd1-115">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="56dd1-115">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="56dd1-116">Criar um novo objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="56dd1-116">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="56dd1-117">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="56dd1-117">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="56dd1-118">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="56dd1-118">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="56dd1-119">Leia as propriedades e os relacionamentos de um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="56dd1-119">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="56dd1-120">Update</span><span class="sxs-lookup"><span data-stu-id="56dd1-120">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="56dd1-121">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="56dd1-121">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="56dd1-122">Atualizar um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="56dd1-122">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="56dd1-123">Delete</span><span class="sxs-lookup"><span data-stu-id="56dd1-123">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="56dd1-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56dd1-124">None</span></span> |<span data-ttu-id="56dd1-125">Excluir um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="56dd1-125">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="56dd1-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56dd1-126">Properties</span></span>
| <span data-ttu-id="56dd1-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56dd1-127">Property</span></span>     | <span data-ttu-id="56dd1-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="56dd1-128">Type</span></span>   |<span data-ttu-id="56dd1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="56dd1-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56dd1-130">displayName</span><span class="sxs-lookup"><span data-stu-id="56dd1-130">displayName</span></span>|<span data-ttu-id="56dd1-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56dd1-131">String</span></span>|<span data-ttu-id="56dd1-132">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="56dd1-132">The name of the customer.</span></span>|
|<span data-ttu-id="56dd1-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="56dd1-133">emailAddress</span></span>|<span data-ttu-id="56dd1-134">String</span><span class="sxs-lookup"><span data-stu-id="56dd1-134">String</span></span>|<span data-ttu-id="56dd1-135">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="56dd1-135">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="56dd1-136">id</span><span class="sxs-lookup"><span data-stu-id="56dd1-136">id</span></span>|<span data-ttu-id="56dd1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56dd1-137">String</span></span>| <span data-ttu-id="56dd1-138">A ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="56dd1-138">The ID of the customer.</span></span> <span data-ttu-id="56dd1-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56dd1-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56dd1-140">Relações</span><span class="sxs-lookup"><span data-stu-id="56dd1-140">Relationships</span></span>
<span data-ttu-id="56dd1-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56dd1-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="56dd1-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56dd1-142">JSON representation</span></span>

<span data-ttu-id="56dd1-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56dd1-143">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


