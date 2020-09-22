---
title: tipo de recurso bookingPerson
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 04fabd62ee89c275d25075de7b489e512ebe3167
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071770"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="ee7f7-104">tipo de recurso bookingPerson</span><span class="sxs-lookup"><span data-stu-id="ee7f7-104">bookingPerson resource type</span></span>

<span data-ttu-id="ee7f7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7f7-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="ee7f7-106">Este é um tipo base para uma pessoa em um Microsoft bookings Business, que pode ser um [bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f7-106">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee7f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee7f7-107">Properties</span></span>
| <span data-ttu-id="ee7f7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee7f7-108">Property</span></span>     | <span data-ttu-id="ee7f7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee7f7-109">Type</span></span>   |<span data-ttu-id="ee7f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee7f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee7f7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ee7f7-111">displayName</span></span>|<span data-ttu-id="ee7f7-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee7f7-112">String</span></span>|<span data-ttu-id="ee7f7-113">Um nome para a entidade derivada, que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="ee7f7-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="ee7f7-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ee7f7-114">emailAddress</span></span>|<span data-ttu-id="ee7f7-115">String</span><span class="sxs-lookup"><span data-stu-id="ee7f7-115">String</span></span>|<span data-ttu-id="ee7f7-116">O endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="ee7f7-116">The email address of the person.</span></span>|
|<span data-ttu-id="ee7f7-117">id</span><span class="sxs-lookup"><span data-stu-id="ee7f7-117">id</span></span>|<span data-ttu-id="ee7f7-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee7f7-118">String</span></span>| <span data-ttu-id="ee7f7-119">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="ee7f7-119">The ID for the derived entity.</span></span> <span data-ttu-id="ee7f7-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee7f7-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee7f7-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ee7f7-121">Relationships</span></span>
<span data-ttu-id="ee7f7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee7f7-122">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ee7f7-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee7f7-123">JSON representation</span></span>

<span data-ttu-id="ee7f7-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee7f7-124">The following is a JSON representation of the resource.</span></span>

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


