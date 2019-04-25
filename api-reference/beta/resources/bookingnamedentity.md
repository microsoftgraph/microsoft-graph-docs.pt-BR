---
title: tipo de recurso bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1cee769181fdf8dce694050cdbc2658fdf29ece4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535449"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="537fe-104">tipo de recurso bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="537fe-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="537fe-105">Este é um tipo base para entidades de livros da Microsoft que fornecem um nome de exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="537fe-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="537fe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="537fe-106">Properties</span></span>
| <span data-ttu-id="537fe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="537fe-107">Property</span></span>     | <span data-ttu-id="537fe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="537fe-108">Type</span></span>   |<span data-ttu-id="537fe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="537fe-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="537fe-110">displayName</span><span class="sxs-lookup"><span data-stu-id="537fe-110">displayName</span></span>|<span data-ttu-id="537fe-111">String</span><span class="sxs-lookup"><span data-stu-id="537fe-111">String</span></span>|<span data-ttu-id="537fe-112">Um nome para a entidade derivada, que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="537fe-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="537fe-113">id</span><span class="sxs-lookup"><span data-stu-id="537fe-113">id</span></span>|<span data-ttu-id="537fe-114">String</span><span class="sxs-lookup"><span data-stu-id="537fe-114">String</span></span>| <span data-ttu-id="537fe-115">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="537fe-115">The ID for the derived entity.</span></span> <span data-ttu-id="537fe-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="537fe-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="537fe-117">Relações</span><span class="sxs-lookup"><span data-stu-id="537fe-117">Relationships</span></span>
<span data-ttu-id="537fe-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="537fe-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="537fe-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="537fe-119">JSON representation</span></span>

<span data-ttu-id="537fe-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="537fe-120">The following is a JSON representation of the resource.</span></span>

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
