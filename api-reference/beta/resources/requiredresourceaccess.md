---
title: tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão OAuth 2,0 e funções de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 84641cc49a518eb41095b80aa0501dce5acf3d35
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453100"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="3d11f-103">tipo de recurso requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="3d11f-103">requiredResourceAccess resource type</span></span>

<span data-ttu-id="3d11f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d11f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d11f-105">Especifica o conjunto de escopos de permissão de OAuth 2,0 e funções de aplicativo no recurso especificado que um aplicativo exige acesso.</span><span class="sxs-lookup"><span data-stu-id="3d11f-105">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="3d11f-106">Os escopos de permissão OAuth 2,0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="3d11f-106">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="3d11f-107">A propriedade **requiredResourceAccess** da entidade [Application](application.md) é uma coleção de **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="3d11f-107">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3d11f-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d11f-108">JSON representation</span></span>

<span data-ttu-id="3d11f-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3d11f-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3d11f-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d11f-110">Properties</span></span>
| <span data-ttu-id="3d11f-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d11f-111">Property</span></span>     | <span data-ttu-id="3d11f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d11f-112">Type</span></span>   |<span data-ttu-id="3d11f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d11f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d11f-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="3d11f-114">resourceAccess</span></span>|<span data-ttu-id="3d11f-115">Coleção [ResourceAccess](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="3d11f-115">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="3d11f-116">A lista de escopos de permissão OAuth 2.0 e funções de aplicativo que o aplicativo requer do recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="3d11f-116">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="3d11f-117">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="3d11f-117">resourceAppId</span></span>|<span data-ttu-id="3d11f-118">String</span><span class="sxs-lookup"><span data-stu-id="3d11f-118">String</span></span>|<span data-ttu-id="3d11f-119">O identificador exclusivo do recurso ao qual o aplicativo exige acesso.</span><span class="sxs-lookup"><span data-stu-id="3d11f-119">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="3d11f-120">Isso deve ser igual ao **AppID** declarado no aplicativo de recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="3d11f-120">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
