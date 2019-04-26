---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo. A propriedade **resourceAccess** do tipo requiredResourceAccess é uma coleção de **resourceAccess**.
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563032"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="b5e4d-104">tipo de recurso resourceAccess</span><span class="sxs-lookup"><span data-stu-id="b5e4d-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e4d-105">Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b5e4d-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="b5e4d-106">A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **resourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="b5e4d-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b5e4d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5e4d-107">JSON representation</span></span>

<span data-ttu-id="b5e4d-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b5e4d-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b5e4d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5e4d-109">Properties</span></span>
| <span data-ttu-id="b5e4d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5e4d-110">Property</span></span>     | <span data-ttu-id="b5e4d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5e4d-111">Type</span></span>   |<span data-ttu-id="b5e4d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e4d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5e4d-113">id</span><span class="sxs-lookup"><span data-stu-id="b5e4d-113">id</span></span>|<span data-ttu-id="b5e4d-114">Guid</span><span class="sxs-lookup"><span data-stu-id="b5e4d-114">Guid</span></span>|<span data-ttu-id="b5e4d-115">O identificador exclusivo de uma das instâncias [oAuth2Permission](oauth2permission.md) ou [appRole](approle.md) que o aplicativo de recursos expõe.</span><span class="sxs-lookup"><span data-stu-id="b5e4d-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="b5e4d-116">type</span><span class="sxs-lookup"><span data-stu-id="b5e4d-116">type</span></span>|<span data-ttu-id="b5e4d-117">String</span><span class="sxs-lookup"><span data-stu-id="b5e4d-117">String</span></span>|<span data-ttu-id="b5e4d-118">Especifica se a propriedade **ID** faz referência a um [OAuth2Permission](oauth2permission.md) ou um [appRole](approle.md).</span><span class="sxs-lookup"><span data-stu-id="b5e4d-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="b5e4d-119">Os valores possíveis são "escopo" ou "função".</span><span class="sxs-lookup"><span data-stu-id="b5e4d-119">Possible values are "scope" or "role".</span></span>|

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
