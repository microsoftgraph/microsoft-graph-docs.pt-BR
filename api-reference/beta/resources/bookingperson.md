---
title: tipo de recurso de bookingPerson
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e39fbbf12909e7a4d29c95e22896df081522a7d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990107"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="d1869-104">tipo de recurso de bookingPerson</span><span class="sxs-lookup"><span data-stu-id="d1869-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="d1869-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1869-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1869-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1869-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d1869-107">Este é um tipo de base para uma pessoa de uma empresa Microsoft Bookings, que pode ser um [bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="d1869-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d1869-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1869-108">Properties</span></span>
| <span data-ttu-id="d1869-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1869-109">Property</span></span>     | <span data-ttu-id="d1869-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1869-110">Type</span></span>   |<span data-ttu-id="d1869-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1869-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1869-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d1869-112">displayName</span></span>|<span data-ttu-id="d1869-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1869-113">String</span></span>|<span data-ttu-id="d1869-114">Um nome da entidade derivada, qual interfaces com os clientes.</span><span class="sxs-lookup"><span data-stu-id="d1869-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="d1869-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d1869-115">emailAddress</span></span>|<span data-ttu-id="d1869-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1869-116">String</span></span>|<span data-ttu-id="d1869-117">O endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="d1869-117">The email address of the person.</span></span>|
|<span data-ttu-id="d1869-118">id</span><span class="sxs-lookup"><span data-stu-id="d1869-118">id</span></span>|<span data-ttu-id="d1869-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1869-119">String</span></span>| <span data-ttu-id="d1869-120">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="d1869-120">The ID for the derived entity.</span></span> <span data-ttu-id="d1869-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1869-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1869-122">Relações</span><span class="sxs-lookup"><span data-stu-id="d1869-122">Relationships</span></span>
<span data-ttu-id="d1869-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1869-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d1869-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1869-124">JSON representation</span></span>

<span data-ttu-id="d1869-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1869-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
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
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
