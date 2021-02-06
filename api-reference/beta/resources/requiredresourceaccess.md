---
title: Tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão do OAuth 2.0 e funções de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: f9a847e6863353e59602aef3c794bc7d79e40d5e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133718"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="5dcec-103">Tipo de recurso requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="5dcec-103">requiredResourceAccess resource type</span></span>

<span data-ttu-id="5dcec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dcec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dcec-105">Especifica o conjunto de escopos de permissão OAuth 2.0 e funções de aplicativo sob o recurso especificado que um aplicativo requer acesso.</span><span class="sxs-lookup"><span data-stu-id="5dcec-105">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="5dcec-106">Os escopos de permissão OAuth 2.0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess)** ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="5dcec-106">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="5dcec-107">A **propriedade requiredResourceAccess** da entidade [do](application.md) aplicativo é uma coleção de **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="5dcec-107">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5dcec-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5dcec-108">JSON representation</span></span>

<span data-ttu-id="5dcec-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5dcec-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="5dcec-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5dcec-110">Properties</span></span>
| <span data-ttu-id="5dcec-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dcec-111">Property</span></span>     | <span data-ttu-id="5dcec-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dcec-112">Type</span></span>   |<span data-ttu-id="5dcec-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dcec-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dcec-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="5dcec-114">resourceAccess</span></span>|<span data-ttu-id="5dcec-115">[Coleção ResourceAccess](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="5dcec-115">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="5dcec-116">A lista de escopos de permissão OAuth2.0 e funções de aplicativo que o aplicativo requer do recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="5dcec-116">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="5dcec-117">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="5dcec-117">resourceAppId</span></span>|<span data-ttu-id="5dcec-118">String</span><span class="sxs-lookup"><span data-stu-id="5dcec-118">String</span></span>|<span data-ttu-id="5dcec-119">O identificador exclusivo do recurso ao que o aplicativo exige acesso.</span><span class="sxs-lookup"><span data-stu-id="5dcec-119">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="5dcec-120">Isso deve ser igual à **appId** declarada no aplicativo de recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="5dcec-120">This should be equal to the **appId** declared on the target resource application.</span></span>|

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


