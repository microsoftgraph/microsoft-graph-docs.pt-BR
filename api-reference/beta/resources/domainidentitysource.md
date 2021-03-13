---
title: Tipo de recurso domainIdentitySource
description: O tipo domainIdentitySource identifica um domínio não locatário como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae616c98b2ca20ec4e5d9c7aceeba5bdeb538e81
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759661"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="8669f-103">Tipo de recurso domainIdentitySource</span><span class="sxs-lookup"><span data-stu-id="8669f-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="8669f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8669f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8669f-105">Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="8669f-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="8669f-106">O `@odata.type` valor indica que esse tipo identifica um domínio como uma fonte de identidade para uma organização `#microsoft.graph.domainIdentitySource` conectada.</span><span class="sxs-lookup"><span data-stu-id="8669f-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="8669f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8669f-107">Properties</span></span>

| <span data-ttu-id="8669f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8669f-108">Property</span></span>                     | <span data-ttu-id="8669f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8669f-109">Type</span></span>                      | <span data-ttu-id="8669f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8669f-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="8669f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8669f-111">displayName</span></span> |<span data-ttu-id="8669f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8669f-112">String</span></span> | <span data-ttu-id="8669f-113">O nome da fonte de identidade, normalmente também o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="8669f-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="8669f-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8669f-114">Read only.</span></span> |
| <span data-ttu-id="8669f-115">domainName</span><span class="sxs-lookup"><span data-stu-id="8669f-115">domainName</span></span> |<span data-ttu-id="8669f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8669f-116">String</span></span> | <span data-ttu-id="8669f-117">O nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="8669f-117">The domain name.</span></span> <span data-ttu-id="8669f-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8669f-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8669f-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8669f-119">Relationships</span></span>

<span data-ttu-id="8669f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8669f-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8669f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8669f-121">JSON representation</span></span>

<span data-ttu-id="8669f-122">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="8669f-122">The following is a JSON representation of the type.</span></span>

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


