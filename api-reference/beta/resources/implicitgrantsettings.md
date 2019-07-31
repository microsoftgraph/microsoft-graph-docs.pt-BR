---
title: tipo de recurso implicitGrantSettings
description: Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92ba18488cc2700b565be47bac3874b6d75e1c13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005790"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="1aabb-105">tipo de recurso implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="1aabb-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aabb-106">Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="1aabb-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="1aabb-107">Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito.</span><span class="sxs-lookup"><span data-stu-id="1aabb-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="1aabb-108">Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.</span><span class="sxs-lookup"><span data-stu-id="1aabb-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="1aabb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1aabb-109">Properties</span></span>

| <span data-ttu-id="1aabb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aabb-110">Property</span></span> | <span data-ttu-id="1aabb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aabb-111">Type</span></span> | <span data-ttu-id="1aabb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aabb-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="1aabb-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="1aabb-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="1aabb-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1aabb-114">Boolean</span></span> | <span data-ttu-id="1aabb-115">Especifica se este aplicativo Web pode solicitar um token de ID usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="1aabb-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="1aabb-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="1aabb-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="1aabb-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="1aabb-117">Boolean</span></span> | <span data-ttu-id="1aabb-118">Especifica se este aplicativo Web pode solicitar um token de acesso usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="1aabb-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1aabb-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1aabb-119">JSON representation</span></span>
<span data-ttu-id="1aabb-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1aabb-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
