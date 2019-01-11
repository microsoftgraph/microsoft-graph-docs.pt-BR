---
title: tipo de recurso de bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: fa307d0ee07b43a44210fc6ceaf4c74a29999caa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860498"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="2c9f6-104">tipo de recurso de bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="2c9f6-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="2c9f6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2c9f6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c9f6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c9f6-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="2c9f6-107">Este é um tipo de base para entidades do Microsoft Bookings que fornecem um nome para exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="2c9f6-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c9f6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c9f6-108">Properties</span></span>
| <span data-ttu-id="2c9f6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c9f6-109">Property</span></span>     | <span data-ttu-id="2c9f6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c9f6-110">Type</span></span>   |<span data-ttu-id="2c9f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c9f6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c9f6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2c9f6-112">displayName</span></span>|<span data-ttu-id="2c9f6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c9f6-113">String</span></span>|<span data-ttu-id="2c9f6-114">Um nome da entidade derivada, qual interfaces com os clientes.</span><span class="sxs-lookup"><span data-stu-id="2c9f6-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="2c9f6-115">id</span><span class="sxs-lookup"><span data-stu-id="2c9f6-115">id</span></span>|<span data-ttu-id="2c9f6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c9f6-116">String</span></span>| <span data-ttu-id="2c9f6-117">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="2c9f6-117">The ID for the derived entity.</span></span> <span data-ttu-id="2c9f6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c9f6-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c9f6-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2c9f6-119">Relationships</span></span>
<span data-ttu-id="2c9f6-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c9f6-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2c9f6-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c9f6-121">JSON representation</span></span>

<span data-ttu-id="2c9f6-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c9f6-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
