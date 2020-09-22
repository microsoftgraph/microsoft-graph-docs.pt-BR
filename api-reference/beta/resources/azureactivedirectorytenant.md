---
title: tipo de recurso azureActiveDirectoryTenant
description: O tipo azureActiveDirectoryTenant identifica outro locatário do Azure Active Directory como uma fonte de identidade para uma organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c2fd1b8e1b2fcc2c2fef03db93a54d5d0b69b951
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089767"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="05339-103">tipo de recurso azureActiveDirectoryTenant</span><span class="sxs-lookup"><span data-stu-id="05339-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="05339-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05339-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05339-105">Usado nas fontes de identidade de um [connectedOrganization](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="05339-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="05339-106">O `@odata.type` valor `#microsoft.graph.azureActiveDirectoryTenant` indica que esse tipo identifica outro locatário do Azure Active Directory como uma fonte de identidade para uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="05339-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="05339-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05339-107">Properties</span></span>

| <span data-ttu-id="05339-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05339-108">Property</span></span>                     | <span data-ttu-id="05339-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="05339-109">Type</span></span>                      | <span data-ttu-id="05339-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="05339-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="05339-111">displayName</span><span class="sxs-lookup"><span data-stu-id="05339-111">displayName</span></span> |<span data-ttu-id="05339-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05339-112">String</span></span> | <span data-ttu-id="05339-113">O nome do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="05339-113">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="05339-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05339-114">Read only.</span></span> |
| <span data-ttu-id="05339-115">tenantId</span><span class="sxs-lookup"><span data-stu-id="05339-115">tenantId</span></span> |<span data-ttu-id="05339-116">String</span><span class="sxs-lookup"><span data-stu-id="05339-116">String</span></span> | <span data-ttu-id="05339-117">A ID do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="05339-117">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="05339-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05339-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="05339-119">Relações</span><span class="sxs-lookup"><span data-stu-id="05339-119">Relationships</span></span>

<span data-ttu-id="05339-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05339-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05339-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05339-121">JSON representation</span></span>

<span data-ttu-id="05339-122">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="05339-122">The following is a JSON representation of the type.</span></span>

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


