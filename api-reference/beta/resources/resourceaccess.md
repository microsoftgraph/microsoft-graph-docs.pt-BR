---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d0d04ba99c0132a0f305bb0fdcaa5e32071d7554
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939261"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="6d078-103">tipo de recurso resourceAccess</span><span class="sxs-lookup"><span data-stu-id="6d078-103">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d078-104">Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d078-104">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="6d078-105">A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **resourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="6d078-105">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6d078-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d078-106">JSON representation</span></span>

<span data-ttu-id="6d078-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6d078-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6d078-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d078-108">Properties</span></span>
| <span data-ttu-id="6d078-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d078-109">Property</span></span>     | <span data-ttu-id="6d078-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d078-110">Type</span></span>   |<span data-ttu-id="6d078-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d078-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d078-112">id</span><span class="sxs-lookup"><span data-stu-id="6d078-112">id</span></span>|<span data-ttu-id="6d078-113">Guid</span><span class="sxs-lookup"><span data-stu-id="6d078-113">Guid</span></span>|<span data-ttu-id="6d078-114">O identificador exclusivo de uma das instâncias [oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recursos expõe.</span><span class="sxs-lookup"><span data-stu-id="6d078-114">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="6d078-115">type</span><span class="sxs-lookup"><span data-stu-id="6d078-115">type</span></span>|<span data-ttu-id="6d078-116">String</span><span class="sxs-lookup"><span data-stu-id="6d078-116">String</span></span>|<span data-ttu-id="6d078-117">Especifica se a propriedade **ID** faz referência a um [Oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md).</span><span class="sxs-lookup"><span data-stu-id="6d078-117">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="6d078-118">Os valores possíveis são "escopo" ou "função".</span><span class="sxs-lookup"><span data-stu-id="6d078-118">Possible values are "scope" or "role".</span></span>|

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
