---
title: Tipo de recurso userConsentRequest
description: Uma solicitação criada por um usuário para usar um aplicativo que exige acesso a dados organizacionais que o usuário não tem autorização para conceder consentimento a si mesmo.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a3ac490e4dcd7231c8b005eeb6a259e525bbf882
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698038"
---
# <a name="userconsentrequest-resource-type"></a><span data-ttu-id="af22d-103">Tipo de recurso userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="af22d-103">userConsentRequest resource type</span></span>

<span data-ttu-id="af22d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af22d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af22d-105">Um [userConsentRequest](../resources/userconsentrequest.md) é criado por um usuário quando ele está solicitando acesso a um aplicativo que exige uma autorização de administrador para acessar.</span><span class="sxs-lookup"><span data-stu-id="af22d-105">A [userConsentRequest](../resources/userconsentrequest.md) is created by a user when they are requesting access to an application which requires an admin authorization to access.</span></span> 

## <a name="methods"></a><span data-ttu-id="af22d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="af22d-106">Methods</span></span>

<span data-ttu-id="af22d-107">Método</span><span class="sxs-lookup"><span data-stu-id="af22d-107">Method</span></span>|<span data-ttu-id="af22d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="af22d-108">Return type</span></span>|<span data-ttu-id="af22d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af22d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af22d-110">Listar userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="af22d-110">List userConsentRequests</span></span>](../api/userconsentrequest-list.md)|<span data-ttu-id="af22d-111">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="af22d-111">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="af22d-112">Recupere uma coleção de [objetos userConsentRequest](userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="af22d-112">Retrieve a collection of [userConsentRequest](userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md).</span></span>|
|[<span data-ttu-id="af22d-113">Obter userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="af22d-113">Get userConsentRequest</span></span>](../api/userconsentrequest-get.md)|[<span data-ttu-id="af22d-114">userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="af22d-114">userConsentRequest</span></span>](../resources/userconsentrequest.md)|<span data-ttu-id="af22d-115">Leia as propriedades e as relações de um [objeto userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="af22d-115">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="af22d-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="af22d-116">filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md)|<span data-ttu-id="af22d-117">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="af22d-117">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="af22d-118">Leia as propriedades dos [objetos userConsentRequest](../resources/userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md) para o qual o usuário atual é o revistor.</span><span class="sxs-lookup"><span data-stu-id="af22d-118">Read the properties of [userConsentRequest](../resources/userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md) for which the current user is the reviewer.</span></span>|

## <a name="properties"></a><span data-ttu-id="af22d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af22d-119">Properties</span></span>

|<span data-ttu-id="af22d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af22d-120">Property</span></span>|<span data-ttu-id="af22d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="af22d-121">Type</span></span>|<span data-ttu-id="af22d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="af22d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af22d-123">approvalId</span><span class="sxs-lookup"><span data-stu-id="af22d-123">approvalId</span></span>|<span data-ttu-id="af22d-124">String</span><span class="sxs-lookup"><span data-stu-id="af22d-124">String</span></span>|<span data-ttu-id="af22d-125">A id da aprovação.</span><span class="sxs-lookup"><span data-stu-id="af22d-125">The id of the approval.</span></span> <span data-ttu-id="af22d-126">Esse valor é igual ao valor do `id` .</span><span class="sxs-lookup"><span data-stu-id="af22d-126">This value is equal to the value of the `id`.</span></span>|
|<span data-ttu-id="af22d-127">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="af22d-127">completedDateTime</span></span>|<span data-ttu-id="af22d-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af22d-128">DateTimeOffset</span></span>|<span data-ttu-id="af22d-129">A data e a hora em **que o status** da solicitação foi marcado como `Completed` .</span><span class="sxs-lookup"><span data-stu-id="af22d-129">The date and time when the **status** of the request was marked as `Completed`.</span></span> <span data-ttu-id="af22d-130">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="af22d-130">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="af22d-131">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="af22d-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="af22d-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="af22d-132">createdBy</span></span>|[<span data-ttu-id="af22d-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="af22d-133">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="af22d-134">O usuário que criou a solicitação.</span><span class="sxs-lookup"><span data-stu-id="af22d-134">The user who created the request.</span></span>|
|<span data-ttu-id="af22d-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af22d-135">createdDateTime</span></span>|<span data-ttu-id="af22d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af22d-136">DateTimeOffset</span></span>|<span data-ttu-id="af22d-137">A data e a hora em que a solicitação foi criada.</span><span class="sxs-lookup"><span data-stu-id="af22d-137">The date and time when the request was created.</span></span> <span data-ttu-id="af22d-138">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="af22d-138">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="af22d-139">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="af22d-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="af22d-140">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="af22d-140">Supports `$filter` (`eq` only) and `$orderby`.</span></span>|
|<span data-ttu-id="af22d-141">customData</span><span class="sxs-lookup"><span data-stu-id="af22d-141">customData</span></span>|<span data-ttu-id="af22d-142">String</span><span class="sxs-lookup"><span data-stu-id="af22d-142">String</span></span>|<span data-ttu-id="af22d-143">Campo de texto livre para definir quaisquer dados personalizados para a solicitação de consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="af22d-143">Free text field to define any custom data for the user consent request.</span></span> <span data-ttu-id="af22d-144">Não usado.</span><span class="sxs-lookup"><span data-stu-id="af22d-144">Not used.</span></span>|
|<span data-ttu-id="af22d-145">id</span><span class="sxs-lookup"><span data-stu-id="af22d-145">id</span></span>|<span data-ttu-id="af22d-146">String</span><span class="sxs-lookup"><span data-stu-id="af22d-146">String</span></span>|<span data-ttu-id="af22d-147">Identificador da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af22d-147">Identifier of the request.</span></span> |
|<span data-ttu-id="af22d-148">motivo</span><span class="sxs-lookup"><span data-stu-id="af22d-148">reason</span></span>|<span data-ttu-id="af22d-149">String</span><span class="sxs-lookup"><span data-stu-id="af22d-149">String</span></span>|<span data-ttu-id="af22d-150">A justificativa do usuário para exigir acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af22d-150">The user's justification for requiring access to the app.</span></span> <span data-ttu-id="af22d-151">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="af22d-151">Supports `$filter` (`eq` only) and `$orderby`.</span></span>  |
|<span data-ttu-id="af22d-152">status</span><span class="sxs-lookup"><span data-stu-id="af22d-152">status</span></span>|<span data-ttu-id="af22d-153">String</span><span class="sxs-lookup"><span data-stu-id="af22d-153">String</span></span>|<span data-ttu-id="af22d-154">O status da solicitação de consentimento do aplicativo do usuário.</span><span class="sxs-lookup"><span data-stu-id="af22d-154">The status of the user's app consent request.</span></span> <span data-ttu-id="af22d-155">Os valores possíveis são: `Initializing` `InProgress` , e `Completed` .</span><span class="sxs-lookup"><span data-stu-id="af22d-155">Possible values are: `Initializing`, `InProgress`, and `Completed`.</span></span> <span data-ttu-id="af22d-156">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="af22d-156">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="af22d-157">Relações</span><span class="sxs-lookup"><span data-stu-id="af22d-157">Relationships</span></span>

|<span data-ttu-id="af22d-158">Relação</span><span class="sxs-lookup"><span data-stu-id="af22d-158">Relationship</span></span>|<span data-ttu-id="af22d-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="af22d-159">Type</span></span>|<span data-ttu-id="af22d-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="af22d-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af22d-161">aprovação</span><span class="sxs-lookup"><span data-stu-id="af22d-161">approval</span></span>|[<span data-ttu-id="af22d-162">aprovação</span><span class="sxs-lookup"><span data-stu-id="af22d-162">approval</span></span>](../resources/approval.md)|<span data-ttu-id="af22d-163">Decisões de aprovação associadas a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="af22d-163">Approval decisions associated with a request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af22d-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af22d-164">JSON representation</span></span>

<span data-ttu-id="af22d-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af22d-165">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "reason": "String"
}
```
