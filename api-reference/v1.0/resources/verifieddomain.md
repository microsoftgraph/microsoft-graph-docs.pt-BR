---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
ms.openlocfilehash: 6eb6490ce8dac29f2617b7873230fad7c7b5c536
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876493"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="8a024-104">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="8a024-104">verifiedDomain resource type</span></span>

<span data-ttu-id="8a024-p102">Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="8a024-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="8a024-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a024-107">Properties</span></span>
| <span data-ttu-id="8a024-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a024-108">Property</span></span>     | <span data-ttu-id="8a024-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a024-109">Type</span></span>   |<span data-ttu-id="8a024-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a024-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a024-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="8a024-111">capabilities</span></span>|<span data-ttu-id="8a024-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a024-112">String</span></span>|<span data-ttu-id="8a024-113">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="8a024-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="8a024-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="8a024-114">isDefault</span></span>|<span data-ttu-id="8a024-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a024-115">Boolean</span></span>|                <span data-ttu-id="8a024-116">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="8a024-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="8a024-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="8a024-117">isInitial</span></span>|<span data-ttu-id="8a024-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a024-118">Boolean</span></span>|<span data-ttu-id="8a024-119">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="8a024-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="8a024-120">name</span><span class="sxs-lookup"><span data-stu-id="8a024-120">name</span></span>|<span data-ttu-id="8a024-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a024-121">String</span></span>|<span data-ttu-id="8a024-122">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="8a024-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="8a024-123">type</span><span class="sxs-lookup"><span data-stu-id="8a024-123">type</span></span>|<span data-ttu-id="8a024-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a024-124">String</span></span>|<span data-ttu-id="8a024-125">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="8a024-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a024-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a024-126">JSON representation</span></span>

<span data-ttu-id="8a024-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8a024-127">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
