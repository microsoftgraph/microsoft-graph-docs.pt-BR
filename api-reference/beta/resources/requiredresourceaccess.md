---
title: tipo de recurso de requiredResourceAccess
description: Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado. Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada. A propriedade **requiredResourceAccess** da entidade do aplicativo é uma coleção de **ReqiredResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512966"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="bba9b-105">tipo de recurso de requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="bba9b-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bba9b-106">Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="bba9b-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="bba9b-107">Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada.</span><span class="sxs-lookup"><span data-stu-id="bba9b-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="bba9b-108">A propriedade **requiredResourceAccess** da entidade do [aplicativo](application.md) é uma coleção de **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="bba9b-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bba9b-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bba9b-109">JSON representation</span></span>

<span data-ttu-id="bba9b-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bba9b-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="bba9b-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bba9b-111">Properties</span></span>
| <span data-ttu-id="bba9b-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bba9b-112">Property</span></span>     | <span data-ttu-id="bba9b-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="bba9b-113">Type</span></span>   |<span data-ttu-id="bba9b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="bba9b-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bba9b-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="bba9b-115">resourceAccess</span></span>|<span data-ttu-id="bba9b-116">Coleção [ResourceAccess](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="bba9b-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="bba9b-117">A lista de escopos de permissão OAuth2.0 e funções de aplicativo que requer que o aplicativo do recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="bba9b-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="bba9b-118">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="bba9b-118">resourceAppId</span></span>|<span data-ttu-id="bba9b-119">String</span><span class="sxs-lookup"><span data-stu-id="bba9b-119">String</span></span>|<span data-ttu-id="bba9b-120">O identificador exclusivo para o recurso que o aplicativo exija acesso à.</span><span class="sxs-lookup"><span data-stu-id="bba9b-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="bba9b-121">Este deve ser igual a **appId** declaradas na aplicação de recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="bba9b-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
