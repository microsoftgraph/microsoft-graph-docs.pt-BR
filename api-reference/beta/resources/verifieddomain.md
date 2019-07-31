---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 091bb8e6c1a14f6c173d18acf68679feb6c88eaf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964215"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="7b0ad-104">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="7b0ad-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b0ad-105">Especifica um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="7b0ad-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="7b0ad-106">A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="7b0ad-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="7b0ad-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b0ad-107">Properties</span></span>
| <span data-ttu-id="7b0ad-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b0ad-108">Property</span></span>     | <span data-ttu-id="7b0ad-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b0ad-109">Type</span></span>   |<span data-ttu-id="7b0ad-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b0ad-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b0ad-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="7b0ad-111">capabilities</span></span>|<span data-ttu-id="7b0ad-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b0ad-112">String</span></span>|<span data-ttu-id="7b0ad-113">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="7b0ad-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="7b0ad-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="7b0ad-114">isDefault</span></span>|<span data-ttu-id="7b0ad-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b0ad-115">Boolean</span></span>|                <span data-ttu-id="7b0ad-116">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="7b0ad-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="7b0ad-117">isinitial</span><span class="sxs-lookup"><span data-stu-id="7b0ad-117">isInitial</span></span>|<span data-ttu-id="7b0ad-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b0ad-118">Boolean</span></span>|<span data-ttu-id="7b0ad-119">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="7b0ad-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="7b0ad-120">name</span><span class="sxs-lookup"><span data-stu-id="7b0ad-120">name</span></span>|<span data-ttu-id="7b0ad-121">String</span><span class="sxs-lookup"><span data-stu-id="7b0ad-121">String</span></span>|<span data-ttu-id="7b0ad-122">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="7b0ad-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="7b0ad-123">type</span><span class="sxs-lookup"><span data-stu-id="7b0ad-123">type</span></span>|<span data-ttu-id="7b0ad-124">String</span><span class="sxs-lookup"><span data-stu-id="7b0ad-124">String</span></span>|<span data-ttu-id="7b0ad-125">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="7b0ad-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b0ad-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b0ad-126">JSON representation</span></span>

<span data-ttu-id="7b0ad-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7b0ad-127">Here is a JSON representation of the resource</span></span>

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
