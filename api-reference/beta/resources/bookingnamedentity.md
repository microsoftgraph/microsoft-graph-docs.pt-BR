---
title: tipo de recurso de bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: abd5c9e85357caa6ba6cbbd52d67550a463e36e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985778"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="bdee9-104">tipo de recurso de bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="bdee9-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="bdee9-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bdee9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdee9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bdee9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bdee9-107">Este é um tipo de base para entidades do Microsoft Bookings que fornecem um nome para exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="bdee9-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bdee9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdee9-108">Properties</span></span>
| <span data-ttu-id="bdee9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdee9-109">Property</span></span>     | <span data-ttu-id="bdee9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdee9-110">Type</span></span>   |<span data-ttu-id="bdee9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdee9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdee9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bdee9-112">displayName</span></span>|<span data-ttu-id="bdee9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdee9-113">String</span></span>|<span data-ttu-id="bdee9-114">Um nome da entidade derivada, qual interfaces com os clientes.</span><span class="sxs-lookup"><span data-stu-id="bdee9-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="bdee9-115">id</span><span class="sxs-lookup"><span data-stu-id="bdee9-115">id</span></span>|<span data-ttu-id="bdee9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdee9-116">String</span></span>| <span data-ttu-id="bdee9-117">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="bdee9-117">The ID for the derived entity.</span></span> <span data-ttu-id="bdee9-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdee9-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdee9-119">Relações</span><span class="sxs-lookup"><span data-stu-id="bdee9-119">Relationships</span></span>
<span data-ttu-id="bdee9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdee9-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bdee9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdee9-121">JSON representation</span></span>

<span data-ttu-id="bdee9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdee9-122">The following is a JSON representation of the resource.</span></span>

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
