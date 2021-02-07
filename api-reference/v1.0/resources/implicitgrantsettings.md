---
title: Tipo de recurso implicitGrantSettings
description: Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58509ff0f0264a683aaae9c83d60e0f041ef0af7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133277"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="ab643-105">Tipo de recurso implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="ab643-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="ab643-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab643-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab643-107">Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="ab643-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="ab643-108">Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito.</span><span class="sxs-lookup"><span data-stu-id="ab643-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="ab643-109">Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.</span><span class="sxs-lookup"><span data-stu-id="ab643-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="ab643-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab643-110">Properties</span></span>

| <span data-ttu-id="ab643-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab643-111">Property</span></span> | <span data-ttu-id="ab643-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab643-112">Type</span></span> | <span data-ttu-id="ab643-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab643-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="ab643-114">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="ab643-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="ab643-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab643-115">Boolean</span></span> | <span data-ttu-id="ab643-116">Especifica se esse aplicativo Web pode solicitar um token de ID usando o fluxo implícito do OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="ab643-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="ab643-117">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="ab643-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="ab643-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab643-118">Boolean</span></span> | <span data-ttu-id="ab643-119">Especifica se esse aplicativo Web pode solicitar um token de acesso usando o fluxo implícito do OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="ab643-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab643-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab643-120">JSON representation</span></span>
<span data-ttu-id="ab643-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab643-121">Here is a JSON representation of the resource.</span></span>
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

