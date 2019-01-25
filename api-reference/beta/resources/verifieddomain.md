---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade **organization** é uma coleção de VerifiedDomain.
localization_priority: Normal
ms.openlocfilehash: c13c3b3da39b762c26d637deaddafbee5da40160
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513393"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="6223b-104">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="6223b-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6223b-p102">Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="6223b-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="6223b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6223b-107">Properties</span></span>
| <span data-ttu-id="6223b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6223b-108">Property</span></span>     | <span data-ttu-id="6223b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6223b-109">Type</span></span>   |<span data-ttu-id="6223b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6223b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6223b-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="6223b-111">capabilities</span></span>|<span data-ttu-id="6223b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6223b-112">String</span></span>|<span data-ttu-id="6223b-113">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="6223b-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="6223b-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="6223b-114">isDefault</span></span>|<span data-ttu-id="6223b-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="6223b-115">Boolean</span></span>|                <span data-ttu-id="6223b-116">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="6223b-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="6223b-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="6223b-117">isInitial</span></span>|<span data-ttu-id="6223b-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="6223b-118">Boolean</span></span>|<span data-ttu-id="6223b-119">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="6223b-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="6223b-120">name</span><span class="sxs-lookup"><span data-stu-id="6223b-120">name</span></span>|<span data-ttu-id="6223b-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6223b-121">String</span></span>|<span data-ttu-id="6223b-122">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="6223b-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="6223b-123">type</span><span class="sxs-lookup"><span data-stu-id="6223b-123">type</span></span>|<span data-ttu-id="6223b-124">String</span><span class="sxs-lookup"><span data-stu-id="6223b-124">String</span></span>|<span data-ttu-id="6223b-125">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="6223b-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6223b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6223b-126">JSON representation</span></span>

<span data-ttu-id="6223b-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6223b-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/verifieddomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
