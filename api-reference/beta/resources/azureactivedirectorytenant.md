---
title: Tipo de recurso do azureActiveDirectoryTenant
description: O tipo azureActiveDirectoryTenant identifica outro locatário do Azure Active Directory como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: acd59c82f1968cbb161b74d1e7c1a551b6b2e397
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759906"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="7a71c-103">Tipo de recurso do azureActiveDirectoryTenant</span><span class="sxs-lookup"><span data-stu-id="7a71c-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="7a71c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a71c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a71c-105">Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="7a71c-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="7a71c-106">O valor indica que esse tipo identifica outro locatário do `@odata.type` Azure Active Directory como uma fonte de `#microsoft.graph.azureActiveDirectoryTenant` identidade para uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="7a71c-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="7a71c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a71c-107">Properties</span></span>

| <span data-ttu-id="7a71c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a71c-108">Property</span></span>                     | <span data-ttu-id="7a71c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a71c-109">Type</span></span>                      | <span data-ttu-id="7a71c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a71c-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="7a71c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7a71c-111">displayName</span></span> |<span data-ttu-id="7a71c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a71c-112">String</span></span> | <span data-ttu-id="7a71c-113">O nome do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7a71c-113">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="7a71c-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a71c-114">Read only.</span></span> |
| <span data-ttu-id="7a71c-115">tenantId</span><span class="sxs-lookup"><span data-stu-id="7a71c-115">tenantId</span></span> |<span data-ttu-id="7a71c-116">String</span><span class="sxs-lookup"><span data-stu-id="7a71c-116">String</span></span> | <span data-ttu-id="7a71c-117">A ID do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7a71c-117">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="7a71c-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a71c-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7a71c-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7a71c-119">Relationships</span></span>

<span data-ttu-id="7a71c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a71c-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a71c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a71c-121">JSON representation</span></span>

<span data-ttu-id="7a71c-122">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="7a71c-122">The following is a JSON representation of the type.</span></span>

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


