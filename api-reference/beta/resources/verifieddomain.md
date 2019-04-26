---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
ms.openlocfilehash: 088687d4450a5134c53bca6134039f7ba34a7597
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345077"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="8f90a-104">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="8f90a-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f90a-105">Especifica um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="8f90a-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="8f90a-106">A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="8f90a-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="8f90a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f90a-107">Properties</span></span>
| <span data-ttu-id="8f90a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f90a-108">Property</span></span>     | <span data-ttu-id="8f90a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f90a-109">Type</span></span>   |<span data-ttu-id="8f90a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f90a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f90a-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="8f90a-111">capabilities</span></span>|<span data-ttu-id="8f90a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f90a-112">String</span></span>|<span data-ttu-id="8f90a-113">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="8f90a-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="8f90a-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="8f90a-114">isDefault</span></span>|<span data-ttu-id="8f90a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f90a-115">Boolean</span></span>|                <span data-ttu-id="8f90a-116">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="8f90a-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="8f90a-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="8f90a-117">isInitial</span></span>|<span data-ttu-id="8f90a-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f90a-118">Boolean</span></span>|<span data-ttu-id="8f90a-119">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="8f90a-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="8f90a-120">name</span><span class="sxs-lookup"><span data-stu-id="8f90a-120">name</span></span>|<span data-ttu-id="8f90a-121">String</span><span class="sxs-lookup"><span data-stu-id="8f90a-121">String</span></span>|<span data-ttu-id="8f90a-122">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="8f90a-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="8f90a-123">type</span><span class="sxs-lookup"><span data-stu-id="8f90a-123">type</span></span>|<span data-ttu-id="8f90a-124">String</span><span class="sxs-lookup"><span data-stu-id="8f90a-124">String</span></span>|<span data-ttu-id="8f90a-125">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="8f90a-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f90a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f90a-126">JSON representation</span></span>

<span data-ttu-id="8f90a-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8f90a-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
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
  "suppressions": []
}
-->
