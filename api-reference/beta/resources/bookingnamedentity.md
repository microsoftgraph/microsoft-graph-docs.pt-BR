---
title: tipo de recurso bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5c219d0ab879c1bc1ae172d08322647b2c261497
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507986"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="a0e47-104">tipo de recurso bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="a0e47-104">bookingNamedEntity resource type</span></span>

<span data-ttu-id="a0e47-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a0e47-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a0e47-106">Este é um tipo base para entidades de livros da Microsoft que fornecem um nome de exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="a0e47-106">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a0e47-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0e47-107">Properties</span></span>
| <span data-ttu-id="a0e47-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0e47-108">Property</span></span>     | <span data-ttu-id="a0e47-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0e47-109">Type</span></span>   |<span data-ttu-id="a0e47-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0e47-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0e47-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a0e47-111">displayName</span></span>|<span data-ttu-id="a0e47-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0e47-112">String</span></span>|<span data-ttu-id="a0e47-113">Um nome para a entidade derivada, que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="a0e47-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="a0e47-114">id</span><span class="sxs-lookup"><span data-stu-id="a0e47-114">id</span></span>|<span data-ttu-id="a0e47-115">String</span><span class="sxs-lookup"><span data-stu-id="a0e47-115">String</span></span>| <span data-ttu-id="a0e47-116">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="a0e47-116">The ID for the derived entity.</span></span> <span data-ttu-id="a0e47-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0e47-117">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0e47-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a0e47-118">Relationships</span></span>
<span data-ttu-id="a0e47-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0e47-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a0e47-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0e47-120">JSON representation</span></span>

<span data-ttu-id="a0e47-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0e47-121">The following is a JSON representation of the resource.</span></span>

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
