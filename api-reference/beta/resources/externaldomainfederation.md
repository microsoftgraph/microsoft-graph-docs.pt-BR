---
title: Tipo de recurso externalDomainFederation
description: O tipo externalDomainFederation identifica um domínio não locatário com um provedor de identidade configurado como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df88fef22c2acb86cadcfaed9a8f5be25da70f9d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760985"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="6b20e-103">Tipo de recurso externalDomainFederation</span><span class="sxs-lookup"><span data-stu-id="6b20e-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="6b20e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b20e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b20e-105">Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="6b20e-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="6b20e-106">O valor indica que esse tipo identifica um domínio com um provedor de identidade configurado como uma fonte de `@odata.type` identidade para uma organização `#microsoft.graph.externalDomainFederation` conectada.</span><span class="sxs-lookup"><span data-stu-id="6b20e-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="6b20e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b20e-107">Properties</span></span>

| <span data-ttu-id="6b20e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b20e-108">Property</span></span>                     | <span data-ttu-id="6b20e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b20e-109">Type</span></span>                      | <span data-ttu-id="6b20e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b20e-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="6b20e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6b20e-111">displayName</span></span> |<span data-ttu-id="6b20e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b20e-112">String</span></span> | <span data-ttu-id="6b20e-113">O nome da fonte de identidade, normalmente também o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="6b20e-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="6b20e-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b20e-114">Read only.</span></span> |
| <span data-ttu-id="6b20e-115">domainName</span><span class="sxs-lookup"><span data-stu-id="6b20e-115">domainName</span></span> |<span data-ttu-id="6b20e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b20e-116">String</span></span> | <span data-ttu-id="6b20e-117">O nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="6b20e-117">The domain name.</span></span> <span data-ttu-id="6b20e-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b20e-118">Read only.</span></span> |
| <span data-ttu-id="6b20e-119">issuerUri</span><span class="sxs-lookup"><span data-stu-id="6b20e-119">issuerUri</span></span> |<span data-ttu-id="6b20e-120">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6b20e-120">String</span></span> | <span data-ttu-id="6b20e-121">O emissorURI da federação de entrada.</span><span class="sxs-lookup"><span data-stu-id="6b20e-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="6b20e-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b20e-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6b20e-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6b20e-123">Relationships</span></span>

<span data-ttu-id="6b20e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b20e-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b20e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b20e-125">JSON representation</span></span>

<span data-ttu-id="6b20e-126">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="6b20e-126">The following is a JSON representation of the type.</span></span>

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


