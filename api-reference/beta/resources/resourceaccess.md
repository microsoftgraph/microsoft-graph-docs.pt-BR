---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 1580f6677ddb2e24d457696fb14d3d07d8bb64d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026253"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="acb79-103">tipo de recurso resourceAccess</span><span class="sxs-lookup"><span data-stu-id="acb79-103">resourceAccess resource type</span></span>

<span data-ttu-id="acb79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acb79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acb79-105">Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="acb79-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="acb79-106">A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **resourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="acb79-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>

## <a name="properties"></a><span data-ttu-id="acb79-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acb79-107">Properties</span></span>
| <span data-ttu-id="acb79-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acb79-108">Property</span></span>     | <span data-ttu-id="acb79-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="acb79-109">Type</span></span>   |<span data-ttu-id="acb79-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="acb79-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acb79-111">id</span><span class="sxs-lookup"><span data-stu-id="acb79-111">id</span></span>|<span data-ttu-id="acb79-112">Guid</span><span class="sxs-lookup"><span data-stu-id="acb79-112">Guid</span></span>|<span data-ttu-id="acb79-113">O identificador exclusivo de uma das instâncias [oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recursos expõe.</span><span class="sxs-lookup"><span data-stu-id="acb79-113">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="acb79-114">tipo</span><span class="sxs-lookup"><span data-stu-id="acb79-114">type</span></span>|<span data-ttu-id="acb79-115">String</span><span class="sxs-lookup"><span data-stu-id="acb79-115">String</span></span>|<span data-ttu-id="acb79-116">Especifica se a propriedade **ID** faz referência a um [Oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md).</span><span class="sxs-lookup"><span data-stu-id="acb79-116">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="acb79-117">Os valores possíveis são `Scope` ou `Role` .</span><span class="sxs-lookup"><span data-stu-id="acb79-117">Possible values are `Scope` or `Role`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acb79-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acb79-118">JSON representation</span></span>

<span data-ttu-id="acb79-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acb79-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


