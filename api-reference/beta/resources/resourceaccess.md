---
title: tipo de recurso de resourceAccess
description: Especifica um escopo de permissão do OAuth 2.0 ou uma função do aplicativo que requer um aplicativo. A propriedade **resourceAccess** do tipo requiredResourceAccess é uma coleção de **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519021"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="da235-104">tipo de recurso de resourceAccess</span><span class="sxs-lookup"><span data-stu-id="da235-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da235-105">Especifica um escopo de permissão do OAuth 2.0 ou uma função do aplicativo que requer um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="da235-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="da235-106">A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **ResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="da235-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="da235-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da235-107">JSON representation</span></span>

<span data-ttu-id="da235-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="da235-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="da235-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da235-109">Properties</span></span>
| <span data-ttu-id="da235-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da235-110">Property</span></span>     | <span data-ttu-id="da235-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="da235-111">Type</span></span>   |<span data-ttu-id="da235-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="da235-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da235-113">id</span><span class="sxs-lookup"><span data-stu-id="da235-113">id</span></span>|<span data-ttu-id="da235-114">Guid</span><span class="sxs-lookup"><span data-stu-id="da235-114">Guid</span></span>|<span data-ttu-id="da235-115">O identificador exclusivo para uma das instâncias [oAuth2Permission](oauth2permission.md) ou [appRole](approle.md) que expõe o aplicativo do recurso.</span><span class="sxs-lookup"><span data-stu-id="da235-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="da235-116">type</span><span class="sxs-lookup"><span data-stu-id="da235-116">type</span></span>|<span data-ttu-id="da235-117">String</span><span class="sxs-lookup"><span data-stu-id="da235-117">String</span></span>|<span data-ttu-id="da235-118">Especifica se a propriedade **id** faz referência a um [oAuth2Permission](oauth2permission.md) ou um [appRole](approle.md).</span><span class="sxs-lookup"><span data-stu-id="da235-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="da235-119">Valores possíveis são "escopo" ou "role".</span><span class="sxs-lookup"><span data-stu-id="da235-119">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
