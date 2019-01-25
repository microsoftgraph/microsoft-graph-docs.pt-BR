---
title: tipo de recurso de bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1cee769181fdf8dce694050cdbc2658fdf29ece4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515318"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="607fc-104">tipo de recurso de bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="607fc-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="607fc-105">Este é um tipo de base para entidades do Microsoft Bookings que fornecem um nome para exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="607fc-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="607fc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="607fc-106">Properties</span></span>
| <span data-ttu-id="607fc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="607fc-107">Property</span></span>     | <span data-ttu-id="607fc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="607fc-108">Type</span></span>   |<span data-ttu-id="607fc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="607fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="607fc-110">displayName</span><span class="sxs-lookup"><span data-stu-id="607fc-110">displayName</span></span>|<span data-ttu-id="607fc-111">String</span><span class="sxs-lookup"><span data-stu-id="607fc-111">String</span></span>|<span data-ttu-id="607fc-112">Um nome da entidade derivada, qual interfaces com os clientes.</span><span class="sxs-lookup"><span data-stu-id="607fc-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="607fc-113">id</span><span class="sxs-lookup"><span data-stu-id="607fc-113">id</span></span>|<span data-ttu-id="607fc-114">String</span><span class="sxs-lookup"><span data-stu-id="607fc-114">String</span></span>| <span data-ttu-id="607fc-115">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="607fc-115">The ID for the derived entity.</span></span> <span data-ttu-id="607fc-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="607fc-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="607fc-117">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="607fc-117">Relationships</span></span>
<span data-ttu-id="607fc-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="607fc-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="607fc-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="607fc-119">JSON representation</span></span>

<span data-ttu-id="607fc-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="607fc-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingnamedentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
