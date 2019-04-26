---
title: tipo de recurso bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c9dc533360d28fc470a3a00528a20cea1b7ea551
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328189"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="4b2c3-104">tipo de recurso bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="4b2c3-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="4b2c3-105">Este é um tipo base para entidades de livros da Microsoft que fornecem um nome de exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="4b2c3-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b2c3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b2c3-106">Properties</span></span>
| <span data-ttu-id="4b2c3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b2c3-107">Property</span></span>     | <span data-ttu-id="4b2c3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b2c3-108">Type</span></span>   |<span data-ttu-id="4b2c3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b2c3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b2c3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4b2c3-110">displayName</span></span>|<span data-ttu-id="4b2c3-111">String</span><span class="sxs-lookup"><span data-stu-id="4b2c3-111">String</span></span>|<span data-ttu-id="4b2c3-112">Um nome para a entidade derivada, que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="4b2c3-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="4b2c3-113">id</span><span class="sxs-lookup"><span data-stu-id="4b2c3-113">id</span></span>|<span data-ttu-id="4b2c3-114">String</span><span class="sxs-lookup"><span data-stu-id="4b2c3-114">String</span></span>| <span data-ttu-id="4b2c3-115">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="4b2c3-115">The ID for the derived entity.</span></span> <span data-ttu-id="4b2c3-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4b2c3-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b2c3-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4b2c3-117">Relationships</span></span>
<span data-ttu-id="4b2c3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b2c3-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4b2c3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b2c3-119">JSON representation</span></span>

<span data-ttu-id="4b2c3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b2c3-120">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
