---
title: Tipo de recurso appConsentRequest
description: Uma solicitação que representa uma coleção de objetos userConsentRequest para um aplicativo específico.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d9c01fd4e752bca0fe9518553f52312e523da3a3
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697898"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="f1133-103">Tipo de recurso appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f1133-103">appConsentRequest resource type</span></span>

<span data-ttu-id="f1133-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1133-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1133-105">Uma coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="f1133-105">A collection of [userConsentRequest](../resources/userconsentrequest.md) objects for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="f1133-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f1133-106">Methods</span></span>
|<span data-ttu-id="f1133-107">Método</span><span class="sxs-lookup"><span data-stu-id="f1133-107">Method</span></span>|<span data-ttu-id="f1133-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f1133-108">Return type</span></span>|<span data-ttu-id="f1133-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1133-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f1133-110">Listar appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="f1133-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="f1133-111">[Coleção appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f1133-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="f1133-112">Recupere uma coleção de [objetos appConsentRequest](appconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f1133-112">Retrieve a collection of [appConsentRequest](appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="f1133-113">Obter appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f1133-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="f1133-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f1133-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="f1133-115">Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f1133-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="f1133-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="f1133-116">filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="f1133-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f1133-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="f1133-118">Leia as propriedades dos [objetos appConsentRequest](../resources/appconsentrequest.md) para os quais o usuário atual é o revistor e o status da solicitação de consentimento do usuário é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="f1133-118">Read the properties of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the user consent request is `InProgress`.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1133-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1133-119">Properties</span></span>
|<span data-ttu-id="f1133-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1133-120">Property</span></span>|<span data-ttu-id="f1133-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1133-121">Type</span></span>|<span data-ttu-id="f1133-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1133-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1133-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1133-123">appDisplayName</span></span>|<span data-ttu-id="f1133-124">String</span><span class="sxs-lookup"><span data-stu-id="f1133-124">String</span></span>|<span data-ttu-id="f1133-125">O nome de exibição do aplicativo para o qual o consentimento é solicitado.</span><span class="sxs-lookup"><span data-stu-id="f1133-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="f1133-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1133-126">Required.</span></span> <span data-ttu-id="f1133-127">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="f1133-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="f1133-128">appId</span><span class="sxs-lookup"><span data-stu-id="f1133-128">appId</span></span>|<span data-ttu-id="f1133-129">String</span><span class="sxs-lookup"><span data-stu-id="f1133-129">String</span></span>|<span data-ttu-id="f1133-130">O identificador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1133-130">The identifier of the application.</span></span> <span data-ttu-id="f1133-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1133-131">Required.</span></span> <span data-ttu-id="f1133-132">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="f1133-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="f1133-133">consentType</span><span class="sxs-lookup"><span data-stu-id="f1133-133">consentType</span></span>|<span data-ttu-id="f1133-134">String</span><span class="sxs-lookup"><span data-stu-id="f1133-134">String</span></span>|<span data-ttu-id="f1133-135">O tipo de consentimento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1133-135">The consent type of the request.</span></span> <span data-ttu-id="f1133-136">Os valores possíveis são: `Static`   e  `Dynamic` .</span><span class="sxs-lookup"><span data-stu-id="f1133-136">Possible values are: `Static` and `Dynamic`.</span></span> <span data-ttu-id="f1133-137">Elas representam permissões estáticas e dinâmicas, respectivamente, solicitadas no fluxo de trabalho de consentimento.</span><span class="sxs-lookup"><span data-stu-id="f1133-137">These represent static and dynamic permissions, respectively, requested in the consent workflow.</span></span> <span data-ttu-id="f1133-138">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="f1133-138">Supports `$filter` (`eq` only) and `$orderby`.</span></span> <span data-ttu-id="f1133-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1133-139">Required.</span></span>|
|<span data-ttu-id="f1133-140">id</span><span class="sxs-lookup"><span data-stu-id="f1133-140">id</span></span>|<span data-ttu-id="f1133-141">String</span><span class="sxs-lookup"><span data-stu-id="f1133-141">String</span></span>|<span data-ttu-id="f1133-142">O identificador da solicitação de consentimento do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1133-142">The identifier of the app consent request.</span></span> <span data-ttu-id="f1133-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1133-143">Required.</span></span>|
|<span data-ttu-id="f1133-144">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="f1133-144">pendingScopes</span></span>|<span data-ttu-id="f1133-145">[Coleção appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="f1133-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="f1133-146">Uma lista de escopos pendentes aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="f1133-146">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="f1133-147">Isso será vazio se o consentType for `Static` .</span><span class="sxs-lookup"><span data-stu-id="f1133-147">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="f1133-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1133-148">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1133-149">Relações</span><span class="sxs-lookup"><span data-stu-id="f1133-149">Relationships</span></span>
|<span data-ttu-id="f1133-150">Relação</span><span class="sxs-lookup"><span data-stu-id="f1133-150">Relationship</span></span>|<span data-ttu-id="f1133-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1133-151">Type</span></span>|<span data-ttu-id="f1133-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1133-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1133-153">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="f1133-153">userConsentRequests</span></span>|<span data-ttu-id="f1133-154">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f1133-154">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="f1133-155">Uma lista de solicitações pendentes de consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1133-155">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1133-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1133-156">JSON representation</span></span>
<span data-ttu-id="f1133-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1133-157">The following is a JSON representation of the resource.</span></span>
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

