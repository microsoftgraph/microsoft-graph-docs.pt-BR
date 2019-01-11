---
title: tipo de recurso de resourceAccess
description: Especifica um escopo de permissão do OAuth 2.0 ou uma função do aplicativo que requer um aplicativo. A propriedade **resourceAccess** do tipo requiredResourceAccess é uma coleção de **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: f5389915897c3aab8b8277a45b54042bc861b290
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862332"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="76590-104">tipo de recurso de resourceAccess</span><span class="sxs-lookup"><span data-stu-id="76590-104">resourceAccess resource type</span></span>

> <span data-ttu-id="76590-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="76590-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76590-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76590-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76590-107">Especifica um escopo de permissão do OAuth 2.0 ou uma função do aplicativo que requer um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="76590-107">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="76590-108">A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **ResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="76590-108">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="76590-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76590-109">JSON representation</span></span>

<span data-ttu-id="76590-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="76590-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="76590-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76590-111">Properties</span></span>
| <span data-ttu-id="76590-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76590-112">Property</span></span>     | <span data-ttu-id="76590-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="76590-113">Type</span></span>   |<span data-ttu-id="76590-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="76590-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76590-115">id</span><span class="sxs-lookup"><span data-stu-id="76590-115">id</span></span>|<span data-ttu-id="76590-116">Guid</span><span class="sxs-lookup"><span data-stu-id="76590-116">Guid</span></span>|<span data-ttu-id="76590-117">O identificador exclusivo para uma das instâncias [oAuth2Permission](oauth2permission.md) ou [appRole](approle.md) que expõe o aplicativo do recurso.</span><span class="sxs-lookup"><span data-stu-id="76590-117">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="76590-118">type</span><span class="sxs-lookup"><span data-stu-id="76590-118">type</span></span>|<span data-ttu-id="76590-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76590-119">String</span></span>|<span data-ttu-id="76590-120">Especifica se a propriedade **id** faz referência a um [oAuth2Permission](oauth2permission.md) ou um [appRole](approle.md).</span><span class="sxs-lookup"><span data-stu-id="76590-120">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="76590-121">Valores possíveis são "escopo" ou "role".</span><span class="sxs-lookup"><span data-stu-id="76590-121">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
