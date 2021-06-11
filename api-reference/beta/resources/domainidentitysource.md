---
title: Tipo de recurso domainIdentitySource
description: O tipo domainIdentitySource identifica um domínio não locatário como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2c558213b7198da65eaacdbf0ac42915f3638c56
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896169"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="1f7c3-103">Tipo de recurso domainIdentitySource</span><span class="sxs-lookup"><span data-stu-id="1f7c3-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="1f7c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f7c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f7c3-105">Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="1f7c3-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="1f7c3-106">O `@odata.type` valor indica que esse tipo identifica um domínio como uma fonte de identidade para uma organização `#microsoft.graph.domainIdentitySource` conectada.</span><span class="sxs-lookup"><span data-stu-id="1f7c3-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

<span data-ttu-id="1f7c3-107">Ao criar uma nova [connectedOrganization](../api/connectedorganization-post.md), se o chamador fornece na coleção identitySources um domainIdentitySource e o domínio corresponde a um domínio registrado de um locatário do Azure Active Directory, a organização conectada resultante criada terá uma coleção identitySources contendo um único membro do tipo [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)</span><span class="sxs-lookup"><span data-stu-id="1f7c3-107">When [creating a new connectedOrganization](../api/connectedorganization-post.md), if the caller provides in the identitySources collection a domainIdentitySource and the domain corresponds to a registered domain of an Azure Active Directory tenant, then the resulting connectedOrganization that is created will have an identitySources collection containing a single member of the [azureActiveDirectoryTenant](azureactivedirectorytenant.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="1f7c3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f7c3-108">Properties</span></span>

| <span data-ttu-id="1f7c3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f7c3-109">Property</span></span>                     | <span data-ttu-id="1f7c3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f7c3-110">Type</span></span>                      | <span data-ttu-id="1f7c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f7c3-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="1f7c3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1f7c3-112">displayName</span></span> |<span data-ttu-id="1f7c3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f7c3-113">String</span></span> | <span data-ttu-id="1f7c3-114">O nome da fonte de identidade, normalmente também o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="1f7c3-114">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="1f7c3-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f7c3-115">Read only.</span></span> |
| <span data-ttu-id="1f7c3-116">domainName</span><span class="sxs-lookup"><span data-stu-id="1f7c3-116">domainName</span></span> |<span data-ttu-id="1f7c3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f7c3-117">String</span></span> | <span data-ttu-id="1f7c3-118">O nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="1f7c3-118">The domain name.</span></span> <span data-ttu-id="1f7c3-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f7c3-119">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1f7c3-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1f7c3-120">Relationships</span></span>

<span data-ttu-id="1f7c3-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f7c3-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f7c3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f7c3-122">JSON representation</span></span>

<span data-ttu-id="1f7c3-123">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="1f7c3-123">The following is a JSON representation of the type.</span></span>

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


