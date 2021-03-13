---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 0072bf231fe8dba66b34188952804083593afaa1
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761069"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="9a935-103">tipo de recurso resourceAccess</span><span class="sxs-lookup"><span data-stu-id="9a935-103">resourceAccess resource type</span></span>

<span data-ttu-id="9a935-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a935-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a935-105">Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer.</span><span class="sxs-lookup"><span data-stu-id="9a935-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="9a935-106">A **propriedade resourceAccess** do [tipo requiredResourceAccess](requiredresourceaccess.md) é uma coleção **de ResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="9a935-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>

## <a name="properties"></a><span data-ttu-id="9a935-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a935-107">Properties</span></span>
| <span data-ttu-id="9a935-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a935-108">Property</span></span>     | <span data-ttu-id="9a935-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a935-109">Type</span></span>   |<span data-ttu-id="9a935-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a935-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a935-111">id</span><span class="sxs-lookup"><span data-stu-id="9a935-111">id</span></span>|<span data-ttu-id="9a935-112">Guid</span><span class="sxs-lookup"><span data-stu-id="9a935-112">Guid</span></span>|<span data-ttu-id="9a935-113">O identificador exclusivo de uma das [instâncias oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recurso expõe.</span><span class="sxs-lookup"><span data-stu-id="9a935-113">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="9a935-114">tipo</span><span class="sxs-lookup"><span data-stu-id="9a935-114">type</span></span>|<span data-ttu-id="9a935-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a935-115">String</span></span>|<span data-ttu-id="9a935-116">Especifica se a **propriedade id** faz referência a [um oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md).</span><span class="sxs-lookup"><span data-stu-id="9a935-116">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="9a935-117">Os valores possíveis são: `Scope` ou `Role`.</span><span class="sxs-lookup"><span data-stu-id="9a935-117">Possible values are `Scope` or `Role`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a935-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a935-118">JSON representation</span></span>

<span data-ttu-id="9a935-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a935-119">The following is a JSON representation of the resource.</span></span>

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


