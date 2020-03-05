---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 20766f236bc3f9d8702a257fa3073a4fa205ce51
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446769"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="49705-104">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="49705-104">verifiedDomain resource type</span></span>

<span data-ttu-id="49705-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="49705-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49705-106">Especifica um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="49705-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="49705-107">A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="49705-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="49705-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49705-108">Properties</span></span>
| <span data-ttu-id="49705-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49705-109">Property</span></span>     | <span data-ttu-id="49705-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="49705-110">Type</span></span>   |<span data-ttu-id="49705-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="49705-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49705-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="49705-112">capabilities</span></span>|<span data-ttu-id="49705-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49705-113">String</span></span>|<span data-ttu-id="49705-114">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="49705-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="49705-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="49705-115">isDefault</span></span>|<span data-ttu-id="49705-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="49705-116">Boolean</span></span>|                <span data-ttu-id="49705-117">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="49705-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="49705-118">isinitial</span><span class="sxs-lookup"><span data-stu-id="49705-118">isInitial</span></span>|<span data-ttu-id="49705-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="49705-119">Boolean</span></span>|<span data-ttu-id="49705-120">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="49705-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="49705-121">nome</span><span class="sxs-lookup"><span data-stu-id="49705-121">name</span></span>|<span data-ttu-id="49705-122">String</span><span class="sxs-lookup"><span data-stu-id="49705-122">String</span></span>|<span data-ttu-id="49705-123">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="49705-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="49705-124">type</span><span class="sxs-lookup"><span data-stu-id="49705-124">type</span></span>|<span data-ttu-id="49705-125">String</span><span class="sxs-lookup"><span data-stu-id="49705-125">String</span></span>|<span data-ttu-id="49705-126">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="49705-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49705-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49705-127">JSON representation</span></span>

<span data-ttu-id="49705-128">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="49705-128">Here is a JSON representation of the resource</span></span>

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
