---
title: Tipo de recurso appConsentRequest
description: Uma solicitação que representa uma agregação de userConsentRequests para um aplicativo específico.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ac7e9f2ea8e727a285016641bac10ea3d2e38f9b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469504"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="f563a-103">Tipo de recurso appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f563a-103">appConsentRequest resource type</span></span>

<span data-ttu-id="f563a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f563a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f563a-105">Uma agregação de [userConsentRequests](../resources/userconsentrequest.md) para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="f563a-105">An aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="f563a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f563a-106">Methods</span></span>

|<span data-ttu-id="f563a-107">Método</span><span class="sxs-lookup"><span data-stu-id="f563a-107">Method</span></span>|<span data-ttu-id="f563a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f563a-108">Return type</span></span>|<span data-ttu-id="f563a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f563a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f563a-110">Listar appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="f563a-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="f563a-111">[Coleção appConsentRequest](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f563a-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="f563a-112">Obter uma lista dos [objetos appConsentRequest](../resources/appconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f563a-112">Get a list of the [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="f563a-113">Obter appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f563a-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="f563a-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f563a-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="f563a-115">Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f563a-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="f563a-116">appConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="f563a-116">appConsentRequests: filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="f563a-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="f563a-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="f563a-118">Uma lista do [appConsentRequests](../resources/appconsentrequest.md) para o qual o usuário atual é o revistor</span><span class="sxs-lookup"><span data-stu-id="f563a-118">A list of the [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer</span></span>|

## <a name="properties"></a><span data-ttu-id="f563a-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f563a-119">Properties</span></span>

|<span data-ttu-id="f563a-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f563a-120">Property</span></span>|<span data-ttu-id="f563a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f563a-121">Type</span></span>|<span data-ttu-id="f563a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f563a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f563a-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f563a-123">appDisplayName</span></span>|<span data-ttu-id="f563a-124">String</span><span class="sxs-lookup"><span data-stu-id="f563a-124">String</span></span>|<span data-ttu-id="f563a-125">O nome de exibição do aplicativo para o qual o consentimento é solicitado.</span><span class="sxs-lookup"><span data-stu-id="f563a-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="f563a-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f563a-126">Required.</span></span> <span data-ttu-id="f563a-127">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="f563a-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="f563a-128">appId</span><span class="sxs-lookup"><span data-stu-id="f563a-128">appId</span></span>|<span data-ttu-id="f563a-129">String</span><span class="sxs-lookup"><span data-stu-id="f563a-129">String</span></span>|<span data-ttu-id="f563a-130">O identificador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f563a-130">The identifier of the application.</span></span> <span data-ttu-id="f563a-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f563a-131">Required.</span></span> <span data-ttu-id="f563a-132">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="f563a-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="f563a-133">id</span><span class="sxs-lookup"><span data-stu-id="f563a-133">id</span></span>|<span data-ttu-id="f563a-134">String</span><span class="sxs-lookup"><span data-stu-id="f563a-134">String</span></span>|<span data-ttu-id="f563a-135">O identificador da solicitação de consentimento do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f563a-135">The identifier of the app consent request.</span></span> <span data-ttu-id="f563a-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f563a-136">Required.</span></span>|
|<span data-ttu-id="f563a-137">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="f563a-137">pendingScopes</span></span>|<span data-ttu-id="f563a-138">[Coleção appConsentRequestScope](../resources/appconsentrequestscope.md)</span><span class="sxs-lookup"><span data-stu-id="f563a-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="f563a-139">Uma lista de escopos pendentes aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="f563a-139">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="f563a-140">Isso será vazio se o consentType for `Static` .</span><span class="sxs-lookup"><span data-stu-id="f563a-140">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="f563a-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f563a-141">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f563a-142">Relações</span><span class="sxs-lookup"><span data-stu-id="f563a-142">Relationships</span></span>

|<span data-ttu-id="f563a-143">Relação</span><span class="sxs-lookup"><span data-stu-id="f563a-143">Relationship</span></span>|<span data-ttu-id="f563a-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="f563a-144">Type</span></span>|<span data-ttu-id="f563a-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="f563a-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f563a-146">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="f563a-146">userConsentRequests</span></span>|<span data-ttu-id="f563a-147">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f563a-147">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="f563a-148">Uma lista de solicitações pendentes de consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="f563a-148">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f563a-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f563a-149">JSON representation</span></span>

<span data-ttu-id="f563a-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f563a-150">The following is a JSON representation of the resource.</span></span>
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
