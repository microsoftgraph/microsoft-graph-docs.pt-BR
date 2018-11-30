---
title: tipo de recurso de requiredResourceAccess
description: Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado. Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada. A propriedade **requiredResourceAccess** da entidade do aplicativo é uma coleção de **ReqiredResourceAccess**.
ms.openlocfilehash: 937557f2f078ade1b336cfd00cd128d428d59cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039187"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="2acfc-105">tipo de recurso de requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="2acfc-105">requiredResourceAccess resource type</span></span>

> <span data-ttu-id="2acfc-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2acfc-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2acfc-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2acfc-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2acfc-108">Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="2acfc-108">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="2acfc-109">Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada.</span><span class="sxs-lookup"><span data-stu-id="2acfc-109">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="2acfc-110">A propriedade **requiredResourceAccess** da entidade do [aplicativo](application.md) é uma coleção de **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="2acfc-110">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2acfc-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2acfc-111">JSON representation</span></span>

<span data-ttu-id="2acfc-112">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2acfc-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2acfc-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2acfc-113">Properties</span></span>
| <span data-ttu-id="2acfc-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2acfc-114">Property</span></span>     | <span data-ttu-id="2acfc-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2acfc-115">Type</span></span>   |<span data-ttu-id="2acfc-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2acfc-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2acfc-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="2acfc-117">resourceAccess</span></span>|<span data-ttu-id="2acfc-118">Coleção [ResourceAccess](resourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="2acfc-118">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="2acfc-119">A lista de escopos de permissão OAuth2.0 e funções de aplicativo que requer que o aplicativo do recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="2acfc-119">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="2acfc-120">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="2acfc-120">resourceAppId</span></span>|<span data-ttu-id="2acfc-121">String</span><span class="sxs-lookup"><span data-stu-id="2acfc-121">String</span></span>|<span data-ttu-id="2acfc-122">O identificador exclusivo para o recurso que o aplicativo exija acesso à.</span><span class="sxs-lookup"><span data-stu-id="2acfc-122">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="2acfc-123">Este deve ser igual a **appId** declaradas na aplicação de recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="2acfc-123">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
