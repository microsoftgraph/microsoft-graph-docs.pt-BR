---
title: tipo de recurso de bookingPerson
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: be00e59e2378c454cd9c939f992376dd9c54c3b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508402"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="704a2-104">tipo de recurso de bookingPerson</span><span class="sxs-lookup"><span data-stu-id="704a2-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="704a2-105">Este é um tipo de base para uma pessoa de uma empresa Microsoft Bookings, que pode ser um [bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="704a2-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="704a2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="704a2-106">Properties</span></span>
| <span data-ttu-id="704a2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="704a2-107">Property</span></span>     | <span data-ttu-id="704a2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="704a2-108">Type</span></span>   |<span data-ttu-id="704a2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="704a2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="704a2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="704a2-110">displayName</span></span>|<span data-ttu-id="704a2-111">String</span><span class="sxs-lookup"><span data-stu-id="704a2-111">String</span></span>|<span data-ttu-id="704a2-112">Um nome da entidade derivada, qual interfaces com os clientes.</span><span class="sxs-lookup"><span data-stu-id="704a2-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="704a2-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="704a2-113">emailAddress</span></span>|<span data-ttu-id="704a2-114">String</span><span class="sxs-lookup"><span data-stu-id="704a2-114">String</span></span>|<span data-ttu-id="704a2-115">O endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="704a2-115">The email address of the person.</span></span>|
|<span data-ttu-id="704a2-116">id</span><span class="sxs-lookup"><span data-stu-id="704a2-116">id</span></span>|<span data-ttu-id="704a2-117">String</span><span class="sxs-lookup"><span data-stu-id="704a2-117">String</span></span>| <span data-ttu-id="704a2-118">A ID da entidade derivada.</span><span class="sxs-lookup"><span data-stu-id="704a2-118">The ID for the derived entity.</span></span> <span data-ttu-id="704a2-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="704a2-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="704a2-120">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="704a2-120">Relationships</span></span>
<span data-ttu-id="704a2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="704a2-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="704a2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="704a2-122">JSON representation</span></span>

<span data-ttu-id="704a2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="704a2-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingperson.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
