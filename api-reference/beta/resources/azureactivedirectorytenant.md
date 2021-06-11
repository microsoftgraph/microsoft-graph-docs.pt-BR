---
title: Tipo de recurso do azureActiveDirectoryTenant
description: O tipo azureActiveDirectoryTenant identifica outro locatário Azure Active Directory como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d7a36c8c737866b20585518e1dc34e6944c97885
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896582"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="80cab-103">Tipo de recurso do azureActiveDirectoryTenant</span><span class="sxs-lookup"><span data-stu-id="80cab-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="80cab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80cab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80cab-105">Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="80cab-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="80cab-106">O valor indica que esse tipo identifica outro locatário Azure Active Directory como uma fonte de `@odata.type` identidade para uma organização `#microsoft.graph.azureActiveDirectoryTenant` conectada.</span><span class="sxs-lookup"><span data-stu-id="80cab-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

<span data-ttu-id="80cab-107">Ao criar uma nova [connectedOrganization](../api/connectedorganization-post.md), se o chamador fornece na coleção identitySources um domainIdentitySource e o domínio corresponde a um domínio registrado de um locatário do Azure Active Directory, a organização conectada resultante criada terá uma coleção identitySources contendo um único membro do tipo [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)</span><span class="sxs-lookup"><span data-stu-id="80cab-107">When [creating a new connectedOrganization](../api/connectedorganization-post.md), if the caller provides in the identitySources collection a domainIdentitySource and the domain corresponds to a registered domain of an Azure Active Directory tenant, then the resulting connectedOrganization that is created will have an identitySources collection containing a single member of the [azureActiveDirectoryTenant](azureactivedirectorytenant.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="80cab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80cab-108">Properties</span></span>

| <span data-ttu-id="80cab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80cab-109">Property</span></span>                     | <span data-ttu-id="80cab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="80cab-110">Type</span></span>                      | <span data-ttu-id="80cab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="80cab-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="80cab-112">displayName</span><span class="sxs-lookup"><span data-stu-id="80cab-112">displayName</span></span> |<span data-ttu-id="80cab-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80cab-113">String</span></span> | <span data-ttu-id="80cab-114">O nome do Azure Active Directory locatário.</span><span class="sxs-lookup"><span data-stu-id="80cab-114">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="80cab-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80cab-115">Read only.</span></span> |
| <span data-ttu-id="80cab-116">tenantId</span><span class="sxs-lookup"><span data-stu-id="80cab-116">tenantId</span></span> |<span data-ttu-id="80cab-117">String</span><span class="sxs-lookup"><span data-stu-id="80cab-117">String</span></span> | <span data-ttu-id="80cab-118">A ID do Azure Active Directory locatário.</span><span class="sxs-lookup"><span data-stu-id="80cab-118">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="80cab-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80cab-119">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="80cab-120">Relações</span><span class="sxs-lookup"><span data-stu-id="80cab-120">Relationships</span></span>

<span data-ttu-id="80cab-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80cab-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80cab-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80cab-122">JSON representation</span></span>

<span data-ttu-id="80cab-123">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="80cab-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


