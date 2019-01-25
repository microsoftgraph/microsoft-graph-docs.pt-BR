---
title: tipo de recurso de bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522214"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="8f9f9-104">tipo de recurso de bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8f9f9-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="8f9f9-105">Representa um cliente de um [bookingBsiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8f9f9-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="8f9f9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8f9f9-106">Methods</span></span>

| <span data-ttu-id="8f9f9-107">Método</span><span class="sxs-lookup"><span data-stu-id="8f9f9-107">Method</span></span>           | <span data-ttu-id="8f9f9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8f9f9-108">Return Type</span></span>    |<span data-ttu-id="8f9f9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f9f9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f9f9-110">Clientes de lista</span><span class="sxs-lookup"><span data-stu-id="8f9f9-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="8f9f9-111">coleção [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="8f9f9-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="8f9f9-112">Obtenha uma lista de objetos **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8f9f9-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="8f9f9-113">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8f9f9-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="8f9f9-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8f9f9-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="8f9f9-115">Crie um novo objeto de **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8f9f9-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="8f9f9-116">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8f9f9-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="8f9f9-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8f9f9-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="8f9f9-118">Leia as propriedades e relacionamentos de um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8f9f9-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="8f9f9-119">Update</span><span class="sxs-lookup"><span data-stu-id="8f9f9-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="8f9f9-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8f9f9-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="8f9f9-121">Atualize um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8f9f9-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="8f9f9-122">Delete</span><span class="sxs-lookup"><span data-stu-id="8f9f9-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="8f9f9-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f9f9-123">None</span></span> |<span data-ttu-id="8f9f9-124">Exclua um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8f9f9-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f9f9-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f9f9-125">Properties</span></span>
| <span data-ttu-id="8f9f9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f9f9-126">Property</span></span>     | <span data-ttu-id="8f9f9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f9f9-127">Type</span></span>   |<span data-ttu-id="8f9f9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f9f9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f9f9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="8f9f9-129">displayName</span></span>|<span data-ttu-id="8f9f9-130">String</span><span class="sxs-lookup"><span data-stu-id="8f9f9-130">String</span></span>|<span data-ttu-id="8f9f9-131">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="8f9f9-131">The name of the customer.</span></span>|
|<span data-ttu-id="8f9f9-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8f9f9-132">emailAddress</span></span>|<span data-ttu-id="8f9f9-133">String</span><span class="sxs-lookup"><span data-stu-id="8f9f9-133">String</span></span>|<span data-ttu-id="8f9f9-134">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="8f9f9-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="8f9f9-135">id</span><span class="sxs-lookup"><span data-stu-id="8f9f9-135">id</span></span>|<span data-ttu-id="8f9f9-136">String</span><span class="sxs-lookup"><span data-stu-id="8f9f9-136">String</span></span>| <span data-ttu-id="8f9f9-137">A identificação do cliente.</span><span class="sxs-lookup"><span data-stu-id="8f9f9-137">The ID of the customer.</span></span> <span data-ttu-id="8f9f9-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f9f9-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f9f9-139">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="8f9f9-139">Relationships</span></span>
<span data-ttu-id="8f9f9-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f9f9-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f9f9-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f9f9-141">JSON representation</span></span>

<span data-ttu-id="8f9f9-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f9f9-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
