---
title: tipo de recurso bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 42ad0826cdabbba2c3b26101d93160f71344fc6c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453651"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="7b05d-104">tipo de recurso bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="7b05d-104">bookingCustomer resource type</span></span>

<span data-ttu-id="7b05d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b05d-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="7b05d-106">Representa um cliente de um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="7b05d-106">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="7b05d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b05d-107">Methods</span></span>

| <span data-ttu-id="7b05d-108">Método</span><span class="sxs-lookup"><span data-stu-id="7b05d-108">Method</span></span>           | <span data-ttu-id="7b05d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b05d-109">Return Type</span></span>    |<span data-ttu-id="7b05d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b05d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b05d-111">Listar clientes</span><span class="sxs-lookup"><span data-stu-id="7b05d-111">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="7b05d-112">coleção [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="7b05d-112">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="7b05d-113">Obtenha uma lista de objetos **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="7b05d-113">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="7b05d-114">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="7b05d-114">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="7b05d-115">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="7b05d-115">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="7b05d-116">Criar um novo objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="7b05d-116">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="7b05d-117">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="7b05d-117">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="7b05d-118">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="7b05d-118">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="7b05d-119">Leia as propriedades e os relacionamentos de um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="7b05d-119">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="7b05d-120">Update</span><span class="sxs-lookup"><span data-stu-id="7b05d-120">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="7b05d-121">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="7b05d-121">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="7b05d-122">Atualizar um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="7b05d-122">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="7b05d-123">Delete</span><span class="sxs-lookup"><span data-stu-id="7b05d-123">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="7b05d-124">None</span><span class="sxs-lookup"><span data-stu-id="7b05d-124">None</span></span> |<span data-ttu-id="7b05d-125">Excluir um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="7b05d-125">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7b05d-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b05d-126">Properties</span></span>
| <span data-ttu-id="7b05d-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b05d-127">Property</span></span>     | <span data-ttu-id="7b05d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b05d-128">Type</span></span>   |<span data-ttu-id="7b05d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b05d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b05d-130">displayName</span><span class="sxs-lookup"><span data-stu-id="7b05d-130">displayName</span></span>|<span data-ttu-id="7b05d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b05d-131">String</span></span>|<span data-ttu-id="7b05d-132">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="7b05d-132">The name of the customer.</span></span>|
|<span data-ttu-id="7b05d-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7b05d-133">emailAddress</span></span>|<span data-ttu-id="7b05d-134">String</span><span class="sxs-lookup"><span data-stu-id="7b05d-134">String</span></span>|<span data-ttu-id="7b05d-135">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="7b05d-135">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="7b05d-136">id</span><span class="sxs-lookup"><span data-stu-id="7b05d-136">id</span></span>|<span data-ttu-id="7b05d-137">String</span><span class="sxs-lookup"><span data-stu-id="7b05d-137">String</span></span>| <span data-ttu-id="7b05d-138">A ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="7b05d-138">The ID of the customer.</span></span> <span data-ttu-id="7b05d-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b05d-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b05d-140">Relações</span><span class="sxs-lookup"><span data-stu-id="7b05d-140">Relationships</span></span>
<span data-ttu-id="7b05d-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b05d-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7b05d-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b05d-142">JSON representation</span></span>

<span data-ttu-id="7b05d-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b05d-143">The following is a JSON representation of the resource.</span></span>

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
