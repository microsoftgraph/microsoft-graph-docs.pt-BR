---
title: tipo de recurso externalDomainFederation
description: O tipo externalDomainFederation identifica um domínio sem locatários com um provedor de identidade configurado como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d81255a3687bf3d6aafe9369f901b209f5827b77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026912"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="2b23b-103">tipo de recurso externalDomainFederation</span><span class="sxs-lookup"><span data-stu-id="2b23b-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="2b23b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b23b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b23b-105">Usado nas fontes de identidade de um [connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="2b23b-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="2b23b-106">O `@odata.type` valor `#microsoft.graph.externalDomainFederation` indica que esse tipo identifica um domínio com um provedor de identidade configurado como uma fonte de identidade para uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="2b23b-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="2b23b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b23b-107">Properties</span></span>

| <span data-ttu-id="2b23b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b23b-108">Property</span></span>                     | <span data-ttu-id="2b23b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b23b-109">Type</span></span>                      | <span data-ttu-id="2b23b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b23b-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="2b23b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2b23b-111">displayName</span></span> |<span data-ttu-id="2b23b-112">String</span><span class="sxs-lookup"><span data-stu-id="2b23b-112">String</span></span> | <span data-ttu-id="2b23b-113">O nome da fonte de identidade, normalmente também o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="2b23b-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="2b23b-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b23b-114">Read only.</span></span> |
| <span data-ttu-id="2b23b-115">domainName</span><span class="sxs-lookup"><span data-stu-id="2b23b-115">domainName</span></span> |<span data-ttu-id="2b23b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b23b-116">String</span></span> | <span data-ttu-id="2b23b-117">O nome do domínio.</span><span class="sxs-lookup"><span data-stu-id="2b23b-117">The domain name.</span></span> <span data-ttu-id="2b23b-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b23b-118">Read only.</span></span> |
| <span data-ttu-id="2b23b-119">issuerUri</span><span class="sxs-lookup"><span data-stu-id="2b23b-119">issuerUri</span></span> |<span data-ttu-id="2b23b-120">String</span><span class="sxs-lookup"><span data-stu-id="2b23b-120">String</span></span> | <span data-ttu-id="2b23b-121">O issuerURI da Federação de entrada.</span><span class="sxs-lookup"><span data-stu-id="2b23b-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="2b23b-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b23b-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2b23b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="2b23b-123">Relationships</span></span>

<span data-ttu-id="2b23b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b23b-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b23b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b23b-125">JSON representation</span></span>

<span data-ttu-id="2b23b-126">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="2b23b-126">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalDomainFederation",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String",
  "issuerUri": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalDomainFederation resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


