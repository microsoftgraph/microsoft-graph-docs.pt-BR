---
title: tipo de recurso de bookingPerson
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: d20f6ee9e14723a80f012cfffb1e4b8214f89739
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038100"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="26b3e-104">tipo de recurso de bookingPerson</span><span class="sxs-lookup"><span data-stu-id="26b3e-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="26b3e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="26b3e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26b3e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26b3e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="26b3e-107">Este é um tipo de base para uma pessoa de uma empresa Microsoft Bookings, que pode ser um [bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="26b3e-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="26b3e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26b3e-108">Properties</span></span>
| <span data-ttu-id="26b3e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26b3e-109">Property</span></span>     | <span data-ttu-id="26b3e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="26b3e-110">Type</span></span>   |<span data-ttu-id="26b3e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26b3e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26b3e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="26b3e-112">displayName</span></span>|<span data-ttu-id="26b3e-113">String</span><span class="sxs-lookup"><span data-stu-id="26b3e-113">String</span></span>|<span data-ttu-id="26b3e-114">Um nome da entidade derivada, qual interfaces com os clientes.</span><span class="sxs-lookup"><span data-stu-id="26b3e-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="26b3e-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="26b3e-115">emailAddress</span></span>|<span data-ttu-id="26b3e-116">String</span><span class="sxs-lookup"><span data-stu-id="26b3e-116">String</span></span>|<span data-ttu-id="26b3e-117">O endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="26b3e-117">The email address of the person.</span></span>|
|<span data-ttu-id="26b3e-118">id</span><span class="sxs-lookup"><span data-stu-id="26b3e-118">id</span></span>|<span data-ttu-id="26b3e-119">String</span><span class="sxs-lookup"><span data-stu-id="26b3e-119">String</span></span>| <span data-ttu-id="26b3e-120">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="26b3e-120">The ID for the derived entity.</span></span> <span data-ttu-id="26b3e-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26b3e-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26b3e-122">Relações</span><span class="sxs-lookup"><span data-stu-id="26b3e-122">Relationships</span></span>
<span data-ttu-id="26b3e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26b3e-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="26b3e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26b3e-124">JSON representation</span></span>

<span data-ttu-id="26b3e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26b3e-125">The following is a JSON representation of the resource.</span></span>

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