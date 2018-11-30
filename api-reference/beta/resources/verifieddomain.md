---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
ms.openlocfilehash: 810b5fea0fbaf82eeb452c0f5c6032679590ff49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038429"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="c0304-104">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="c0304-104">verifiedDomain resource type</span></span>

> <span data-ttu-id="c0304-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0304-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0304-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0304-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0304-p103">Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="c0304-p103">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="c0304-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0304-109">Properties</span></span>
| <span data-ttu-id="c0304-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0304-110">Property</span></span>     | <span data-ttu-id="c0304-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0304-111">Type</span></span>   |<span data-ttu-id="c0304-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0304-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0304-113">capabilities</span><span class="sxs-lookup"><span data-stu-id="c0304-113">capabilities</span></span>|<span data-ttu-id="c0304-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0304-114">String</span></span>|<span data-ttu-id="c0304-115">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="c0304-115">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="c0304-116">isDefault</span><span class="sxs-lookup"><span data-stu-id="c0304-116">isDefault</span></span>|<span data-ttu-id="c0304-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0304-117">Boolean</span></span>|                <span data-ttu-id="c0304-118">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="c0304-118">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="c0304-119">isInitial</span><span class="sxs-lookup"><span data-stu-id="c0304-119">isInitial</span></span>|<span data-ttu-id="c0304-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0304-120">Boolean</span></span>|<span data-ttu-id="c0304-121">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="c0304-121">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="c0304-122">name</span><span class="sxs-lookup"><span data-stu-id="c0304-122">name</span></span>|<span data-ttu-id="c0304-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0304-123">String</span></span>|<span data-ttu-id="c0304-124">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="c0304-124">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="c0304-125">type</span><span class="sxs-lookup"><span data-stu-id="c0304-125">type</span></span>|<span data-ttu-id="c0304-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0304-126">String</span></span>|<span data-ttu-id="c0304-127">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="c0304-127">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0304-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0304-128">JSON representation</span></span>

<span data-ttu-id="c0304-129">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c0304-129">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
