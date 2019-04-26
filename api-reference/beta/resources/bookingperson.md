---
title: tipo de recurso bookingPerson
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b4f69fde11ce0717e7ac81bd2070d08cbb59a84a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338751"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="e70da-104">tipo de recurso bookingPerson</span><span class="sxs-lookup"><span data-stu-id="e70da-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e70da-105">Este é um tipo base para uma pessoa em um Microsoft bookings Business, que pode ser um [bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="e70da-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e70da-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e70da-106">Properties</span></span>
| <span data-ttu-id="e70da-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e70da-107">Property</span></span>     | <span data-ttu-id="e70da-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e70da-108">Type</span></span>   |<span data-ttu-id="e70da-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e70da-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e70da-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e70da-110">displayName</span></span>|<span data-ttu-id="e70da-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e70da-111">String</span></span>|<span data-ttu-id="e70da-112">Um nome para a entidade derivada, que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="e70da-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="e70da-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e70da-113">emailAddress</span></span>|<span data-ttu-id="e70da-114">String</span><span class="sxs-lookup"><span data-stu-id="e70da-114">String</span></span>|<span data-ttu-id="e70da-115">O endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="e70da-115">The email address of the person.</span></span>|
|<span data-ttu-id="e70da-116">id</span><span class="sxs-lookup"><span data-stu-id="e70da-116">id</span></span>|<span data-ttu-id="e70da-117">String</span><span class="sxs-lookup"><span data-stu-id="e70da-117">String</span></span>| <span data-ttu-id="e70da-118">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="e70da-118">The ID for the derived entity.</span></span> <span data-ttu-id="e70da-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e70da-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e70da-120">Relações</span><span class="sxs-lookup"><span data-stu-id="e70da-120">Relationships</span></span>
<span data-ttu-id="e70da-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e70da-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e70da-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e70da-122">JSON representation</span></span>

<span data-ttu-id="e70da-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e70da-123">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
