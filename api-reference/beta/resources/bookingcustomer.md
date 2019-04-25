---
title: tipo de recurso bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543861"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="dcade-104">tipo de recurso bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="dcade-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="dcade-105">Representa um cliente de um [bookingBsiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="dcade-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="dcade-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dcade-106">Methods</span></span>

| <span data-ttu-id="dcade-107">Método</span><span class="sxs-lookup"><span data-stu-id="dcade-107">Method</span></span>           | <span data-ttu-id="dcade-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dcade-108">Return Type</span></span>    |<span data-ttu-id="dcade-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcade-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dcade-110">Listar clientes</span><span class="sxs-lookup"><span data-stu-id="dcade-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="dcade-111">coleção [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="dcade-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="dcade-112">Obtenha uma lista de objetos **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="dcade-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="dcade-113">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="dcade-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="dcade-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="dcade-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="dcade-115">Criar um novo objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="dcade-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="dcade-116">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="dcade-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="dcade-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="dcade-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="dcade-118">Leia as propriedades e os relacionamentos de um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="dcade-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="dcade-119">Update</span><span class="sxs-lookup"><span data-stu-id="dcade-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="dcade-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="dcade-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="dcade-121">Atualizar um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="dcade-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="dcade-122">Excluir</span><span class="sxs-lookup"><span data-stu-id="dcade-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="dcade-123">None</span><span class="sxs-lookup"><span data-stu-id="dcade-123">None</span></span> |<span data-ttu-id="dcade-124">Excluir um objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="dcade-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dcade-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dcade-125">Properties</span></span>
| <span data-ttu-id="dcade-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dcade-126">Property</span></span>     | <span data-ttu-id="dcade-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcade-127">Type</span></span>   |<span data-ttu-id="dcade-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcade-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcade-129">displayName</span><span class="sxs-lookup"><span data-stu-id="dcade-129">displayName</span></span>|<span data-ttu-id="dcade-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcade-130">String</span></span>|<span data-ttu-id="dcade-131">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="dcade-131">The name of the customer.</span></span>|
|<span data-ttu-id="dcade-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="dcade-132">emailAddress</span></span>|<span data-ttu-id="dcade-133">String</span><span class="sxs-lookup"><span data-stu-id="dcade-133">String</span></span>|<span data-ttu-id="dcade-134">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="dcade-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="dcade-135">id</span><span class="sxs-lookup"><span data-stu-id="dcade-135">id</span></span>|<span data-ttu-id="dcade-136">String</span><span class="sxs-lookup"><span data-stu-id="dcade-136">String</span></span>| <span data-ttu-id="dcade-137">A ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="dcade-137">The ID of the customer.</span></span> <span data-ttu-id="dcade-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dcade-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcade-139">Relações</span><span class="sxs-lookup"><span data-stu-id="dcade-139">Relationships</span></span>
<span data-ttu-id="dcade-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dcade-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dcade-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dcade-141">JSON representation</span></span>

<span data-ttu-id="dcade-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dcade-142">The following is a JSON representation of the resource.</span></span>

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
