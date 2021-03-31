---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: b4a3a5bed105fe0e0849ddf7c21d7a1b087942ca
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468678"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="17e3f-104">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="17e3f-104">verifiedDomain resource type</span></span>

<span data-ttu-id="17e3f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17e3f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17e3f-106">Especifica um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="17e3f-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="17e3f-107">A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="17e3f-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="17e3f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17e3f-108">Properties</span></span>
| <span data-ttu-id="17e3f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17e3f-109">Property</span></span>     | <span data-ttu-id="17e3f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="17e3f-110">Type</span></span>   |<span data-ttu-id="17e3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="17e3f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17e3f-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="17e3f-112">capabilities</span></span>|<span data-ttu-id="17e3f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17e3f-113">String</span></span>|<span data-ttu-id="17e3f-114">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="17e3f-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="17e3f-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="17e3f-115">isDefault</span></span>|<span data-ttu-id="17e3f-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="17e3f-116">Boolean</span></span>|                <span data-ttu-id="17e3f-117">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="17e3f-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="17e3f-118">isInitial</span><span class="sxs-lookup"><span data-stu-id="17e3f-118">isInitial</span></span>|<span data-ttu-id="17e3f-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="17e3f-119">Boolean</span></span>|<span data-ttu-id="17e3f-120">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="17e3f-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="17e3f-121">nome</span><span class="sxs-lookup"><span data-stu-id="17e3f-121">name</span></span>|<span data-ttu-id="17e3f-122">String</span><span class="sxs-lookup"><span data-stu-id="17e3f-122">String</span></span>|<span data-ttu-id="17e3f-123">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="17e3f-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="17e3f-124">tipo</span><span class="sxs-lookup"><span data-stu-id="17e3f-124">type</span></span>|<span data-ttu-id="17e3f-125">String</span><span class="sxs-lookup"><span data-stu-id="17e3f-125">String</span></span>|<span data-ttu-id="17e3f-126">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="17e3f-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17e3f-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17e3f-127">JSON representation</span></span>

<span data-ttu-id="17e3f-128">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="17e3f-128">Here is a JSON representation of the resource</span></span>

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


