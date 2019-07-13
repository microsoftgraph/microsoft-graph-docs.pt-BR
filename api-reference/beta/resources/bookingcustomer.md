---
title: tipo de recurso bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d996c5e06c5c12e3a5115253bb73ed4a7a450258
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645210"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="ca958-104">tipo de recurso bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="ca958-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="ca958-105">Representa um cliente de um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="ca958-105">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="ca958-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ca958-106">Methods</span></span>

| <span data-ttu-id="ca958-107">Método</span><span class="sxs-lookup"><span data-stu-id="ca958-107">Method</span></span>           | <span data-ttu-id="ca958-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ca958-108">Return Type</span></span>    |<span data-ttu-id="ca958-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca958-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca958-110">Listar clientes</span><span class="sxs-lookup"><span data-stu-id="ca958-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="ca958-111">coleção [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="ca958-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="ca958-112">Obtenha uma lista de objetos **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="ca958-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="ca958-113">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="ca958-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="ca958-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="ca958-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="ca958-115">Criar um novo objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="ca958-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="ca958-116">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="ca958-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="ca958-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="ca958-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="ca958-118">Leia as propriedades e os relacionamentos de um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="ca958-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="ca958-119">Atualização</span><span class="sxs-lookup"><span data-stu-id="ca958-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="ca958-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="ca958-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="ca958-121">Atualizar um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="ca958-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="ca958-122">Delete</span><span class="sxs-lookup"><span data-stu-id="ca958-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="ca958-123">None</span><span class="sxs-lookup"><span data-stu-id="ca958-123">None</span></span> |<span data-ttu-id="ca958-124">Excluir um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="ca958-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca958-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca958-125">Properties</span></span>
| <span data-ttu-id="ca958-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca958-126">Property</span></span>     | <span data-ttu-id="ca958-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca958-127">Type</span></span>   |<span data-ttu-id="ca958-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca958-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca958-129">displayName</span><span class="sxs-lookup"><span data-stu-id="ca958-129">displayName</span></span>|<span data-ttu-id="ca958-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca958-130">String</span></span>|<span data-ttu-id="ca958-131">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="ca958-131">The name of the customer.</span></span>|
|<span data-ttu-id="ca958-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ca958-132">emailAddress</span></span>|<span data-ttu-id="ca958-133">String</span><span class="sxs-lookup"><span data-stu-id="ca958-133">String</span></span>|<span data-ttu-id="ca958-134">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="ca958-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="ca958-135">id</span><span class="sxs-lookup"><span data-stu-id="ca958-135">id</span></span>|<span data-ttu-id="ca958-136">String</span><span class="sxs-lookup"><span data-stu-id="ca958-136">String</span></span>| <span data-ttu-id="ca958-137">A ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="ca958-137">The ID of the customer.</span></span> <span data-ttu-id="ca958-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca958-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca958-139">Relações</span><span class="sxs-lookup"><span data-stu-id="ca958-139">Relationships</span></span>
<span data-ttu-id="ca958-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca958-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ca958-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca958-141">JSON representation</span></span>

<span data-ttu-id="ca958-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca958-142">The following is a JSON representation of the resource.</span></span>

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
