---
title: tipo de recurso bookingPerson
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d5ebbd7c4abaf34b31ac3f3d8e75defd6c939ec0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453657"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="07230-104">tipo de recurso bookingPerson</span><span class="sxs-lookup"><span data-stu-id="07230-104">bookingPerson resource type</span></span>

<span data-ttu-id="07230-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07230-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="07230-106">Este é um tipo base para uma pessoa em um Microsoft bookings Business, que pode ser um [bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="07230-106">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="07230-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07230-107">Properties</span></span>
| <span data-ttu-id="07230-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07230-108">Property</span></span>     | <span data-ttu-id="07230-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="07230-109">Type</span></span>   |<span data-ttu-id="07230-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07230-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07230-111">displayName</span><span class="sxs-lookup"><span data-stu-id="07230-111">displayName</span></span>|<span data-ttu-id="07230-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07230-112">String</span></span>|<span data-ttu-id="07230-113">Um nome para a entidade derivada, que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="07230-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="07230-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="07230-114">emailAddress</span></span>|<span data-ttu-id="07230-115">String</span><span class="sxs-lookup"><span data-stu-id="07230-115">String</span></span>|<span data-ttu-id="07230-116">O endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="07230-116">The email address of the person.</span></span>|
|<span data-ttu-id="07230-117">id</span><span class="sxs-lookup"><span data-stu-id="07230-117">id</span></span>|<span data-ttu-id="07230-118">String</span><span class="sxs-lookup"><span data-stu-id="07230-118">String</span></span>| <span data-ttu-id="07230-119">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="07230-119">The ID for the derived entity.</span></span> <span data-ttu-id="07230-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="07230-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07230-121">Relações</span><span class="sxs-lookup"><span data-stu-id="07230-121">Relationships</span></span>
<span data-ttu-id="07230-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07230-122">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="07230-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07230-123">JSON representation</span></span>

<span data-ttu-id="07230-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07230-124">The following is a JSON representation of the resource.</span></span>

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
