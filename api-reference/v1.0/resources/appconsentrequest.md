---
title: Tipo de recurso appConsentRequest
description: Uma solicitação que representa uma coleção de objetos userConsentRequest para um aplicativo específico.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 32744ce01f871c82a52710502e7fdc899537cef5
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698010"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="b49da-103">Tipo de recurso appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="b49da-103">appConsentRequest resource type</span></span>

<span data-ttu-id="b49da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b49da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b49da-105">Uma coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="b49da-105">A collection of [userConsentRequest](../resources/userconsentrequest.md) objects for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="b49da-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b49da-106">Methods</span></span>

|<span data-ttu-id="b49da-107">Método</span><span class="sxs-lookup"><span data-stu-id="b49da-107">Method</span></span>|<span data-ttu-id="b49da-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b49da-108">Return type</span></span>|<span data-ttu-id="b49da-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b49da-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b49da-110">Listar appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="b49da-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="b49da-111">[Coleção appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b49da-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="b49da-112">Recupere uma coleção de [objetos appConsentRequest](appconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b49da-112">Retrieve a collection of [appConsentRequest](appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="b49da-113">Obter appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="b49da-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="b49da-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="b49da-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="b49da-115">Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b49da-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="b49da-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="b49da-116">filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="b49da-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="b49da-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="b49da-118">Leia as propriedades dos [objetos appConsentRequest](../resources/appconsentrequest.md) para os quais o usuário atual é o revistor e o status da solicitação de consentimento do usuário é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="b49da-118">Read the properties of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the user consent request is `InProgress`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b49da-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b49da-119">Properties</span></span>

|<span data-ttu-id="b49da-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b49da-120">Property</span></span>|<span data-ttu-id="b49da-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b49da-121">Type</span></span>|<span data-ttu-id="b49da-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b49da-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b49da-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="b49da-123">appDisplayName</span></span>|<span data-ttu-id="b49da-124">String</span><span class="sxs-lookup"><span data-stu-id="b49da-124">String</span></span>|<span data-ttu-id="b49da-125">O nome de exibição do aplicativo para o qual o consentimento é solicitado.</span><span class="sxs-lookup"><span data-stu-id="b49da-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="b49da-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b49da-126">Required.</span></span> <span data-ttu-id="b49da-127">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="b49da-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="b49da-128">appId</span><span class="sxs-lookup"><span data-stu-id="b49da-128">appId</span></span>|<span data-ttu-id="b49da-129">String</span><span class="sxs-lookup"><span data-stu-id="b49da-129">String</span></span>|<span data-ttu-id="b49da-130">O identificador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b49da-130">The identifier of the application.</span></span> <span data-ttu-id="b49da-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b49da-131">Required.</span></span> <span data-ttu-id="b49da-132">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="b49da-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="b49da-133">id</span><span class="sxs-lookup"><span data-stu-id="b49da-133">id</span></span>|<span data-ttu-id="b49da-134">String</span><span class="sxs-lookup"><span data-stu-id="b49da-134">String</span></span>|<span data-ttu-id="b49da-135">O identificador da solicitação de consentimento do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b49da-135">The identifier of the app consent request.</span></span> <span data-ttu-id="b49da-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b49da-136">Required.</span></span>|
|<span data-ttu-id="b49da-137">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="b49da-137">pendingScopes</span></span>|<span data-ttu-id="b49da-138">[Coleção appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="b49da-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="b49da-139">Uma lista de escopos pendentes aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="b49da-139">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="b49da-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b49da-140">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b49da-141">Relações</span><span class="sxs-lookup"><span data-stu-id="b49da-141">Relationships</span></span>

|<span data-ttu-id="b49da-142">Relação</span><span class="sxs-lookup"><span data-stu-id="b49da-142">Relationship</span></span>|<span data-ttu-id="b49da-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="b49da-143">Type</span></span>|<span data-ttu-id="b49da-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b49da-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b49da-145">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="b49da-145">userConsentRequests</span></span>|<span data-ttu-id="b49da-146">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b49da-146">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="b49da-147">Uma lista de solicitações pendentes de consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="b49da-147">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b49da-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b49da-148">JSON representation</span></span>

<span data-ttu-id="b49da-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b49da-149">The following is a JSON representation of the resource.</span></span>
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
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```
