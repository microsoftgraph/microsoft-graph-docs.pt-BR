---
title: Tipo de recurso appConsentRequest
description: Uma solicitação que representa uma agregação de userConsentRequests para um aplicativo específico.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f823f64d4c0324aeca74c3268d6fc95d313e2f00
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965060"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="c6be6-103">Tipo de recurso appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="c6be6-103">appConsentRequest resource type</span></span>

<span data-ttu-id="c6be6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6be6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6be6-105">Uma agregação de [userConsentRequests](../resources/userconsentrequest.md) para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="c6be6-105">An aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="c6be6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c6be6-106">Methods</span></span>
|<span data-ttu-id="c6be6-107">Método</span><span class="sxs-lookup"><span data-stu-id="c6be6-107">Method</span></span>|<span data-ttu-id="c6be6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6be6-108">Return type</span></span>|<span data-ttu-id="c6be6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6be6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6be6-110">Listar appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="c6be6-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="c6be6-111">[Coleção appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c6be6-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="c6be6-112">Obter uma lista dos [objetos appConsentRequest](../resources/appconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c6be6-112">Get a list of the [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="c6be6-113">Obter appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="c6be6-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="c6be6-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="c6be6-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="c6be6-115">Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c6be6-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="c6be6-116">Listar appConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="c6be6-116">List appConsentRequests: filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="c6be6-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="c6be6-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="c6be6-118">Uma lista do [appConsentRequests](../resources/appconsentrequest.md) para o qual o usuário atual é o revistor</span><span class="sxs-lookup"><span data-stu-id="c6be6-118">A list of the [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer</span></span>|

## <a name="properties"></a><span data-ttu-id="c6be6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6be6-119">Properties</span></span>
|<span data-ttu-id="c6be6-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6be6-120">Property</span></span>|<span data-ttu-id="c6be6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6be6-121">Type</span></span>|<span data-ttu-id="c6be6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6be6-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6be6-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="c6be6-123">appDisplayName</span></span>|<span data-ttu-id="c6be6-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6be6-124">String</span></span>|<span data-ttu-id="c6be6-125">O nome de exibição do aplicativo para o qual o consentimento é solicitado.</span><span class="sxs-lookup"><span data-stu-id="c6be6-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="c6be6-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6be6-126">Required.</span></span> <span data-ttu-id="c6be6-127">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="c6be6-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="c6be6-128">appId</span><span class="sxs-lookup"><span data-stu-id="c6be6-128">appId</span></span>|<span data-ttu-id="c6be6-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6be6-129">String</span></span>|<span data-ttu-id="c6be6-130">O identificador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6be6-130">The identifier of the application.</span></span> <span data-ttu-id="c6be6-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6be6-131">Required.</span></span> <span data-ttu-id="c6be6-132">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="c6be6-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="c6be6-133">consentType</span><span class="sxs-lookup"><span data-stu-id="c6be6-133">consentType</span></span>|<span data-ttu-id="c6be6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6be6-134">String</span></span>|<span data-ttu-id="c6be6-135">O tipo de consentimento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6be6-135">The consent type of the request.</span></span> <span data-ttu-id="c6be6-136">Os valores possíveis são: `Static`   e  `Dynamic` .</span><span class="sxs-lookup"><span data-stu-id="c6be6-136">Possible values are: `Static` and `Dynamic`.</span></span> <span data-ttu-id="c6be6-137">Elas representam permissões estáticas e dinâmicas, respectivamente, solicitadas no fluxo de trabalho de consentimento.</span><span class="sxs-lookup"><span data-stu-id="c6be6-137">These represent static and dynamic permissions, respectively, requested in the consent workflow.</span></span> <span data-ttu-id="c6be6-138">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="c6be6-138">Supports `$filter` (`eq` only) and `$orderby`.</span></span> <span data-ttu-id="c6be6-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6be6-139">Required.</span></span>|
|<span data-ttu-id="c6be6-140">id</span><span class="sxs-lookup"><span data-stu-id="c6be6-140">id</span></span>|<span data-ttu-id="c6be6-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6be6-141">String</span></span>|<span data-ttu-id="c6be6-142">O identificador da solicitação de consentimento do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6be6-142">The identifier of the app consent request.</span></span> <span data-ttu-id="c6be6-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6be6-143">Required.</span></span>|
|<span data-ttu-id="c6be6-144">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="c6be6-144">pendingScopes</span></span>|<span data-ttu-id="c6be6-145">[Coleção appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="c6be6-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="c6be6-146">Uma lista de escopos pendentes aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="c6be6-146">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="c6be6-147">Isso será vazio se o consentType for `Static` .</span><span class="sxs-lookup"><span data-stu-id="c6be6-147">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="c6be6-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6be6-148">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6be6-149">Relações</span><span class="sxs-lookup"><span data-stu-id="c6be6-149">Relationships</span></span>
|<span data-ttu-id="c6be6-150">Relação</span><span class="sxs-lookup"><span data-stu-id="c6be6-150">Relationship</span></span>|<span data-ttu-id="c6be6-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6be6-151">Type</span></span>|<span data-ttu-id="c6be6-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6be6-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6be6-153">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="c6be6-153">userConsentRequests</span></span>|<span data-ttu-id="c6be6-154">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c6be6-154">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="c6be6-155">Uma lista de solicitações pendentes de consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6be6-155">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6be6-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6be6-156">JSON representation</span></span>
<span data-ttu-id="c6be6-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6be6-157">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "consentType": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```

