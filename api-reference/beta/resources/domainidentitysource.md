---
title: tipo de recurso domainIdentitySource
description: O tipo domainIdentitySource identifica um domínio não-locatário como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 134f0ae3c382c879b48d468545dd40f2d6bd101b
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510033"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="6e85b-103">tipo de recurso domainIdentitySource</span><span class="sxs-lookup"><span data-stu-id="6e85b-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="6e85b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e85b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e85b-105">Usado nas fontes de identidade de um [connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="6e85b-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="6e85b-106">O `@odata.type` valor `#microsoft.graph.domainIdentitySource` indica que esse tipo identifica um domínio como uma fonte de identidade para uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="6e85b-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="6e85b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e85b-107">Properties</span></span>

| <span data-ttu-id="6e85b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e85b-108">Property</span></span>                     | <span data-ttu-id="6e85b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e85b-109">Type</span></span>                      | <span data-ttu-id="6e85b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e85b-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="6e85b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6e85b-111">displayName</span></span> |<span data-ttu-id="6e85b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e85b-112">String</span></span> | <span data-ttu-id="6e85b-113">O nome da fonte de identidade, normalmente também o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="6e85b-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="6e85b-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e85b-114">Read only.</span></span> |
| <span data-ttu-id="6e85b-115">domainName</span><span class="sxs-lookup"><span data-stu-id="6e85b-115">domainName</span></span> |<span data-ttu-id="6e85b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e85b-116">String</span></span> | <span data-ttu-id="6e85b-117">O nome do domínio.</span><span class="sxs-lookup"><span data-stu-id="6e85b-117">The domain name.</span></span> <span data-ttu-id="6e85b-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e85b-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6e85b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6e85b-119">Relationships</span></span>

<span data-ttu-id="6e85b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e85b-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e85b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e85b-121">JSON representation</span></span>

<span data-ttu-id="6e85b-122">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="6e85b-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
