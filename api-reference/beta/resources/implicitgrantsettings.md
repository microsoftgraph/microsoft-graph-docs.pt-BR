---
title: Tipo de recurso implicitGrantSettings
description: 'Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fe471eefe817e48468258195dae4c93331dd6e04
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547012"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="4ce1d-103">Tipo de recurso implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="4ce1d-103">implicitGrantSettings resource type</span></span>

<span data-ttu-id="4ce1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ce1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ce1d-105">Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="4ce1d-105">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="4ce1d-106">Propriedades separadas estão disponíveis para solicitar ID e acessar tokens como parte do fluxo implícito.</span><span class="sxs-lookup"><span data-stu-id="4ce1d-106">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="4ce1d-107">Para habilitar o fluxo implícito, pelo menos uma das seguintes propriedades deve ser definida como true.</span><span class="sxs-lookup"><span data-stu-id="4ce1d-107">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="4ce1d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ce1d-108">Properties</span></span>

| <span data-ttu-id="4ce1d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ce1d-109">Property</span></span> | <span data-ttu-id="4ce1d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ce1d-110">Type</span></span> | <span data-ttu-id="4ce1d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ce1d-111">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="4ce1d-112">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="4ce1d-112">enableIdTokenIssuance</span></span>| <span data-ttu-id="4ce1d-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ce1d-113">Boolean</span></span> | <span data-ttu-id="4ce1d-114">Especifica se esse aplicativo Web pode solicitar um token de ID usando o fluxo implícito OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="4ce1d-114">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="4ce1d-115">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="4ce1d-115">enableAccessTokenIssuance</span></span>| <span data-ttu-id="4ce1d-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ce1d-116">Boolean</span></span> | <span data-ttu-id="4ce1d-117">Especifica se esse aplicativo Web pode solicitar um token de acesso usando o fluxo implícito OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="4ce1d-117">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ce1d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ce1d-118">JSON representation</span></span>
<span data-ttu-id="4ce1d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ce1d-119">Here is a JSON representation of the resource.</span></span>
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


