---
title: tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão de OAuth 2,0 e funções de aplicativo no recurso especificado que um aplicativo exige acesso. Os escopos de permissão OAuth 2,0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** ) ao chamar um aplicativo de recurso. A propriedade **requiredResourceAccess** da entidade Application é uma coleção de **ReqiredResourceAccess**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6c7fec2027e5e987c66f868cc4a69555141bdbf9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965413"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="773b5-105">tipo de recurso requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="773b5-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="773b5-106">Especifica o conjunto de escopos de permissão de OAuth 2,0 e funções de aplicativo no recurso especificado que um aplicativo exige acesso.</span><span class="sxs-lookup"><span data-stu-id="773b5-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="773b5-107">Os escopos de permissão OAuth 2,0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="773b5-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="773b5-108">A propriedade **requiredResourceAccess** da entidade [Application](application.md) é uma coleção de **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="773b5-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="773b5-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="773b5-109">JSON representation</span></span>

<span data-ttu-id="773b5-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="773b5-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="773b5-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="773b5-111">Properties</span></span>
| <span data-ttu-id="773b5-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="773b5-112">Property</span></span>     | <span data-ttu-id="773b5-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="773b5-113">Type</span></span>   |<span data-ttu-id="773b5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="773b5-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="773b5-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="773b5-115">resourceAccess</span></span>|<span data-ttu-id="773b5-116">Coleção [ResourceAccess](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="773b5-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="773b5-117">A lista de escopos de permissão OAuth 2.0 e funções de aplicativo que o aplicativo requer do recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="773b5-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="773b5-118">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="773b5-118">resourceAppId</span></span>|<span data-ttu-id="773b5-119">String</span><span class="sxs-lookup"><span data-stu-id="773b5-119">String</span></span>|<span data-ttu-id="773b5-120">O identificador exclusivo do recurso ao qual o aplicativo exige acesso.</span><span class="sxs-lookup"><span data-stu-id="773b5-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="773b5-121">Isso deve ser igual ao **AppID** declarado no aplicativo de recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="773b5-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

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
