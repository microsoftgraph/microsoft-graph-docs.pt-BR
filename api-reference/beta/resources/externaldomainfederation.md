---
title: tipo de recurso externalDomainFederation
description: O tipo externalDomainFederation identifica um domínio sem locatários com um provedor de identidade configurado como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ffeaa955ac43a52a0e3485f4a561163d4d27a957
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509957"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="f8794-103">tipo de recurso externalDomainFederation</span><span class="sxs-lookup"><span data-stu-id="f8794-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="f8794-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8794-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8794-105">Usado nas fontes de identidade de um [connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="f8794-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="f8794-106">O `@odata.type` valor `#microsoft.graph.externalDomainFederation` indica que esse tipo identifica um domínio com um provedor de identidade configurado como uma fonte de identidade para uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="f8794-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="f8794-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8794-107">Properties</span></span>

| <span data-ttu-id="f8794-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8794-108">Property</span></span>                     | <span data-ttu-id="f8794-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8794-109">Type</span></span>                      | <span data-ttu-id="f8794-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8794-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="f8794-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f8794-111">displayName</span></span> |<span data-ttu-id="f8794-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8794-112">String</span></span> | <span data-ttu-id="f8794-113">O nome da fonte de identidade, normalmente também o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="f8794-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="f8794-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8794-114">Read only.</span></span> |
| <span data-ttu-id="f8794-115">domainName</span><span class="sxs-lookup"><span data-stu-id="f8794-115">domainName</span></span> |<span data-ttu-id="f8794-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8794-116">String</span></span> | <span data-ttu-id="f8794-117">O nome do domínio.</span><span class="sxs-lookup"><span data-stu-id="f8794-117">The domain name.</span></span> <span data-ttu-id="f8794-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8794-118">Read only.</span></span> |
| <span data-ttu-id="f8794-119">issuerUri</span><span class="sxs-lookup"><span data-stu-id="f8794-119">issuerUri</span></span> |<span data-ttu-id="f8794-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8794-120">String</span></span> | <span data-ttu-id="f8794-121">O issuerURI da Federação de entrada.</span><span class="sxs-lookup"><span data-stu-id="f8794-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="f8794-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8794-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f8794-123">Relações</span><span class="sxs-lookup"><span data-stu-id="f8794-123">Relationships</span></span>

<span data-ttu-id="f8794-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8794-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8794-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8794-125">JSON representation</span></span>

<span data-ttu-id="f8794-126">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="f8794-126">The following is a JSON representation of the type.</span></span>

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
