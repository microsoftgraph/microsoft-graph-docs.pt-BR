---
title: tipo de recurso domainIdentitySource
description: O tipo domainIdentitySource identifica um domínio não-locatário como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63301dbf42a4589fd204290c157c6e6f63e473d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010302"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="9d756-103">tipo de recurso domainIdentitySource</span><span class="sxs-lookup"><span data-stu-id="9d756-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="9d756-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d756-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d756-105">Usado nas fontes de identidade de um [connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="9d756-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="9d756-106">O `@odata.type` valor `#microsoft.graph.domainIdentitySource` indica que esse tipo identifica um domínio como uma fonte de identidade para uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="9d756-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="9d756-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d756-107">Properties</span></span>

| <span data-ttu-id="9d756-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d756-108">Property</span></span>                     | <span data-ttu-id="9d756-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d756-109">Type</span></span>                      | <span data-ttu-id="9d756-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d756-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9d756-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9d756-111">displayName</span></span> |<span data-ttu-id="9d756-112">String</span><span class="sxs-lookup"><span data-stu-id="9d756-112">String</span></span> | <span data-ttu-id="9d756-113">O nome da fonte de identidade, normalmente também o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="9d756-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="9d756-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d756-114">Read only.</span></span> |
| <span data-ttu-id="9d756-115">domainName</span><span class="sxs-lookup"><span data-stu-id="9d756-115">domainName</span></span> |<span data-ttu-id="9d756-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d756-116">String</span></span> | <span data-ttu-id="9d756-117">O nome do domínio.</span><span class="sxs-lookup"><span data-stu-id="9d756-117">The domain name.</span></span> <span data-ttu-id="9d756-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d756-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d756-119">Relações</span><span class="sxs-lookup"><span data-stu-id="9d756-119">Relationships</span></span>

<span data-ttu-id="9d756-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d756-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d756-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d756-121">JSON representation</span></span>

<span data-ttu-id="9d756-122">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="9d756-122">The following is a JSON representation of the type.</span></span>

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


