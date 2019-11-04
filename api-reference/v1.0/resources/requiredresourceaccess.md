---
title: tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão OAuth 2,0 e funções de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e6e6577eb6ee23ba430054b43de38fc2dd3a1904
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939790"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="0c180-103">tipo de recurso requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="0c180-103">requiredResourceAccess resource type</span></span>

<span data-ttu-id="0c180-104">Especifica o conjunto de escopos de permissão de OAuth 2,0 e funções de aplicativo no recurso especificado que um aplicativo exige acesso.</span><span class="sxs-lookup"><span data-stu-id="0c180-104">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="0c180-105">Os escopos de permissão OAuth 2,0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="0c180-105">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="0c180-106">A propriedade **requiredResourceAccess** da entidade [Application](application.md) é uma coleção de **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="0c180-106">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c180-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c180-107">JSON representation</span></span>

<span data-ttu-id="0c180-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0c180-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0c180-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c180-109">Properties</span></span>
| <span data-ttu-id="0c180-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c180-110">Property</span></span>     | <span data-ttu-id="0c180-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c180-111">Type</span></span>   |<span data-ttu-id="0c180-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c180-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c180-113">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="0c180-113">resourceAccess</span></span>|<span data-ttu-id="0c180-114">coleção [resourceAccess](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="0c180-114">[resourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="0c180-115">A lista de escopos de permissão OAuth 2.0 e funções de aplicativo que o aplicativo requer do recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="0c180-115">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="0c180-116">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="0c180-116">resourceAppId</span></span>|<span data-ttu-id="0c180-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c180-117">String</span></span>|<span data-ttu-id="0c180-118">O identificador exclusivo do recurso ao qual o aplicativo exige acesso.</span><span class="sxs-lookup"><span data-stu-id="0c180-118">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="0c180-119">Isso deve ser igual ao **AppID** declarado no aplicativo de recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="0c180-119">This should be equal to the **appId** declared on the target resource application.</span></span>|

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
