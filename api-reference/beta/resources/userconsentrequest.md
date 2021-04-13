---
title: Tipo de recurso userConsentRequest
description: Uma solicitação criada por um usuário para usar um aplicativo que exige acesso a dados organizacionais que o usuário não tem autorização para conceder consentimento a si mesmo.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ea9520e34237a0e4b60e5e077a487182b18369e6
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698066"
---
# <a name="userconsentrequest-resource-type"></a><span data-ttu-id="29c99-103">Tipo de recurso userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="29c99-103">userConsentRequest resource type</span></span>

<span data-ttu-id="29c99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29c99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29c99-105">Um [userConsentRequest](../resources/userconsentrequest.md) é criado por um usuário quando ele está solicitando acesso a um aplicativo que exige uma autorização de administrador para acessar.</span><span class="sxs-lookup"><span data-stu-id="29c99-105">A [userConsentRequest](../resources/userconsentrequest.md) is created by a user when they are requesting access to an application which requires an admin authorization to access.</span></span> 

## <a name="methods"></a><span data-ttu-id="29c99-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="29c99-106">Methods</span></span>
|<span data-ttu-id="29c99-107">Método</span><span class="sxs-lookup"><span data-stu-id="29c99-107">Method</span></span>|<span data-ttu-id="29c99-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29c99-108">Return type</span></span>|<span data-ttu-id="29c99-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29c99-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29c99-110">Listar userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="29c99-110">List userConsentRequests</span></span>](../api/userconsentrequest-list.md)|<span data-ttu-id="29c99-111">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="29c99-111">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="29c99-112">Recupere uma coleção de [objetos userConsentRequest](userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="29c99-112">Retrieve a collection of [userConsentRequest](userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md).</span></span>|
|[<span data-ttu-id="29c99-113">Obter userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="29c99-113">Get userConsentRequest</span></span>](../api/userconsentrequest-get.md)|[<span data-ttu-id="29c99-114">userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="29c99-114">userConsentRequest</span></span>](../resources/userconsentrequest.md)|<span data-ttu-id="29c99-115">Leia as propriedades e as relações de um [objeto userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="29c99-115">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="29c99-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="29c99-116">filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md)|<span data-ttu-id="29c99-117">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="29c99-117">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="29c99-118">Leia as propriedades dos [objetos userConsentRequest](../resources/userconsentrequest.md) para [um appConsentRequest](appconsentrequest.md) para o qual o usuário atual é o revistor.</span><span class="sxs-lookup"><span data-stu-id="29c99-118">Read the properties of [userConsentRequest](../resources/userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md) for which the current user is the reviewer.</span></span>|

## <a name="properties"></a><span data-ttu-id="29c99-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29c99-119">Properties</span></span>
|<span data-ttu-id="29c99-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29c99-120">Property</span></span>|<span data-ttu-id="29c99-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="29c99-121">Type</span></span>|<span data-ttu-id="29c99-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="29c99-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29c99-123">approvalId</span><span class="sxs-lookup"><span data-stu-id="29c99-123">approvalId</span></span>|<span data-ttu-id="29c99-124">String</span><span class="sxs-lookup"><span data-stu-id="29c99-124">String</span></span>|<span data-ttu-id="29c99-125">A id da aprovação.</span><span class="sxs-lookup"><span data-stu-id="29c99-125">The id of the approval.</span></span> <span data-ttu-id="29c99-126">Esse valor é igual ao valor do `id` .</span><span class="sxs-lookup"><span data-stu-id="29c99-126">This value is equal to the value of the `id`.</span></span>|
|<span data-ttu-id="29c99-127">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="29c99-127">completedDateTime</span></span>|<span data-ttu-id="29c99-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29c99-128">DateTimeOffset</span></span>|<span data-ttu-id="29c99-129">A data e a hora em **que o status** da solicitação foi marcado como `Completed` .</span><span class="sxs-lookup"><span data-stu-id="29c99-129">The date and time when the **status** of the request was marked as `Completed`.</span></span> <span data-ttu-id="29c99-130">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="29c99-130">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29c99-131">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="29c99-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="29c99-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="29c99-132">createdBy</span></span>|[<span data-ttu-id="29c99-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="29c99-133">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="29c99-134">O usuário que criou a solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c99-134">The user who created the request.</span></span>|
|<span data-ttu-id="29c99-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29c99-135">createdDateTime</span></span>|<span data-ttu-id="29c99-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29c99-136">DateTimeOffset</span></span>|<span data-ttu-id="29c99-137">A data e a hora em que a solicitação foi criada.</span><span class="sxs-lookup"><span data-stu-id="29c99-137">The date and time when the request was created.</span></span> <span data-ttu-id="29c99-138">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="29c99-138">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29c99-139">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="29c99-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="29c99-140">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="29c99-140">Supports `$filter` (`eq` only) and `$orderby`.</span></span>|
|<span data-ttu-id="29c99-141">customData</span><span class="sxs-lookup"><span data-stu-id="29c99-141">customData</span></span>|<span data-ttu-id="29c99-142">String</span><span class="sxs-lookup"><span data-stu-id="29c99-142">String</span></span>|<span data-ttu-id="29c99-143">Campo de texto livre para definir quaisquer dados personalizados para a solicitação de consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="29c99-143">Free text field to define any custom data for the user consent request.</span></span> <span data-ttu-id="29c99-144">Não usado.</span><span class="sxs-lookup"><span data-stu-id="29c99-144">Not used.</span></span>|
|<span data-ttu-id="29c99-145">id</span><span class="sxs-lookup"><span data-stu-id="29c99-145">id</span></span>|<span data-ttu-id="29c99-146">String</span><span class="sxs-lookup"><span data-stu-id="29c99-146">String</span></span>|<span data-ttu-id="29c99-147">Identificador da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c99-147">Identifier of the request.</span></span> |
|<span data-ttu-id="29c99-148">motivo</span><span class="sxs-lookup"><span data-stu-id="29c99-148">reason</span></span>|<span data-ttu-id="29c99-149">String</span><span class="sxs-lookup"><span data-stu-id="29c99-149">String</span></span>|<span data-ttu-id="29c99-150">A justificativa do usuário para exigir acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29c99-150">The user's justification for requiring access to the app.</span></span> <span data-ttu-id="29c99-151">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="29c99-151">Supports `$filter` (`eq` only) and `$orderby`.</span></span>  |
|<span data-ttu-id="29c99-152">status</span><span class="sxs-lookup"><span data-stu-id="29c99-152">status</span></span>|<span data-ttu-id="29c99-153">String</span><span class="sxs-lookup"><span data-stu-id="29c99-153">String</span></span>|<span data-ttu-id="29c99-154">O status da solicitação de consentimento do aplicativo do usuário.</span><span class="sxs-lookup"><span data-stu-id="29c99-154">The status of the user's app consent request.</span></span> <span data-ttu-id="29c99-155">Os valores possíveis são: `Initializing` `InProgress` , e `Completed` .</span><span class="sxs-lookup"><span data-stu-id="29c99-155">Possible values are: `Initializing`, `InProgress`, and `Completed`.</span></span> <span data-ttu-id="29c99-156">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="29c99-156">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="29c99-157">Relações</span><span class="sxs-lookup"><span data-stu-id="29c99-157">Relationships</span></span>
|<span data-ttu-id="29c99-158">Relação</span><span class="sxs-lookup"><span data-stu-id="29c99-158">Relationship</span></span>|<span data-ttu-id="29c99-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="29c99-159">Type</span></span>|<span data-ttu-id="29c99-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="29c99-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29c99-161">aprovação</span><span class="sxs-lookup"><span data-stu-id="29c99-161">approval</span></span>|[<span data-ttu-id="29c99-162">aprovação</span><span class="sxs-lookup"><span data-stu-id="29c99-162">approval</span></span>](../resources/approval.md)|<span data-ttu-id="29c99-163">Decisões de aprovação associadas a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c99-163">Approval decisions associated with a request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29c99-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29c99-164">JSON representation</span></span>
<span data-ttu-id="29c99-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29c99-165">The following is a JSON representation of the resource.</span></span>
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

