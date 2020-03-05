---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 7d369b654a1184470afdefd03aac2103f1a47e01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521100"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="6acce-103">tipo de recurso resourceAccess</span><span class="sxs-lookup"><span data-stu-id="6acce-103">resourceAccess resource type</span></span>

<span data-ttu-id="6acce-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6acce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6acce-105">Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6acce-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="6acce-106">A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **resourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="6acce-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6acce-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6acce-107">JSON representation</span></span>

<span data-ttu-id="6acce-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6acce-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6acce-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6acce-109">Properties</span></span>
| <span data-ttu-id="6acce-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6acce-110">Property</span></span>     | <span data-ttu-id="6acce-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6acce-111">Type</span></span>   |<span data-ttu-id="6acce-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6acce-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6acce-113">id</span><span class="sxs-lookup"><span data-stu-id="6acce-113">id</span></span>|<span data-ttu-id="6acce-114">Guid</span><span class="sxs-lookup"><span data-stu-id="6acce-114">Guid</span></span>|<span data-ttu-id="6acce-115">O identificador exclusivo de uma das instâncias [oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recursos expõe.</span><span class="sxs-lookup"><span data-stu-id="6acce-115">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="6acce-116">type</span><span class="sxs-lookup"><span data-stu-id="6acce-116">type</span></span>|<span data-ttu-id="6acce-117">String</span><span class="sxs-lookup"><span data-stu-id="6acce-117">String</span></span>|<span data-ttu-id="6acce-118">Especifica se a propriedade **ID** faz referência a um [Oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md).</span><span class="sxs-lookup"><span data-stu-id="6acce-118">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="6acce-119">Os valores possíveis são "escopo" ou "função".</span><span class="sxs-lookup"><span data-stu-id="6acce-119">Possible values are "scope" or "role".</span></span>|

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
