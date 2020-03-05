---
title: tipo de recurso implicitGrantSettings
description: Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 97824f704d855d7a2c9b1af84af577a738c3b87a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496478"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="ed822-105">tipo de recurso implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="ed822-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="ed822-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ed822-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed822-107">Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="ed822-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="ed822-108">Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito.</span><span class="sxs-lookup"><span data-stu-id="ed822-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="ed822-109">Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.</span><span class="sxs-lookup"><span data-stu-id="ed822-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="ed822-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed822-110">Properties</span></span>

| <span data-ttu-id="ed822-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed822-111">Property</span></span> | <span data-ttu-id="ed822-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed822-112">Type</span></span> | <span data-ttu-id="ed822-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed822-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="ed822-114">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="ed822-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="ed822-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed822-115">Boolean</span></span> | <span data-ttu-id="ed822-116">Especifica se este aplicativo Web pode solicitar um token de ID usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="ed822-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="ed822-117">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="ed822-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="ed822-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed822-118">Boolean</span></span> | <span data-ttu-id="ed822-119">Especifica se este aplicativo Web pode solicitar um token de acesso usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="ed822-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed822-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed822-120">JSON representation</span></span>
<span data-ttu-id="ed822-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed822-121">Here is a JSON representation of the resource.</span></span>
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
