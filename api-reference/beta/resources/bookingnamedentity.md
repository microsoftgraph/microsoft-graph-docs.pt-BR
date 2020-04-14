---
title: tipo de recurso bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: aa200d2d7aee435f6bb156cc857d471c222e740d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453652"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="0e5b9-104">tipo de recurso bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="0e5b9-104">bookingNamedEntity resource type</span></span>

<span data-ttu-id="0e5b9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e5b9-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="0e5b9-106">Este é um tipo base para entidades de livros da Microsoft que fornecem um nome de exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="0e5b9-106">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0e5b9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e5b9-107">Properties</span></span>
| <span data-ttu-id="0e5b9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e5b9-108">Property</span></span>     | <span data-ttu-id="0e5b9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e5b9-109">Type</span></span>   |<span data-ttu-id="0e5b9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e5b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e5b9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0e5b9-111">displayName</span></span>|<span data-ttu-id="0e5b9-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e5b9-112">String</span></span>|<span data-ttu-id="0e5b9-113">Um nome para a entidade derivada, que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="0e5b9-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="0e5b9-114">id</span><span class="sxs-lookup"><span data-stu-id="0e5b9-114">id</span></span>|<span data-ttu-id="0e5b9-115">String</span><span class="sxs-lookup"><span data-stu-id="0e5b9-115">String</span></span>| <span data-ttu-id="0e5b9-116">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="0e5b9-116">The ID for the derived entity.</span></span> <span data-ttu-id="0e5b9-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e5b9-117">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e5b9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0e5b9-118">Relationships</span></span>
<span data-ttu-id="0e5b9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e5b9-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0e5b9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e5b9-120">JSON representation</span></span>

<span data-ttu-id="0e5b9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e5b9-121">The following is a JSON representation of the resource.</span></span>

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
