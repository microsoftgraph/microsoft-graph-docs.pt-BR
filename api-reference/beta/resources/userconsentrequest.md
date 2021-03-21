---
title: Tipo de recurso userConsentRequest
description: Uma solicitação criada por um usuário para usar um aplicativo que exige acesso a dados organizacionais que o usuário não tem autorização para conceder consentimento a si mesmo.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d3d91688a0a385ea319dee6df90b45c52bd4ec89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965023"
---
# <a name="userconsentrequest-resource-type"></a><span data-ttu-id="ebf37-103">Tipo de recurso userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="ebf37-103">userConsentRequest resource type</span></span>

<span data-ttu-id="ebf37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebf37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebf37-105">Um [userConsentRequest](../resources/userconsentrequest.md) é criado por um usuário quando ele está solicitando acesso a um aplicativo que exige uma autorização de administrador para acessar.</span><span class="sxs-lookup"><span data-stu-id="ebf37-105">A [userConsentRequest](../resources/userconsentrequest.md) is created by an user when they are requesting access to an application which requires an admin authorization to access.</span></span> 

## <a name="methods"></a><span data-ttu-id="ebf37-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ebf37-106">Methods</span></span>
|<span data-ttu-id="ebf37-107">Método</span><span class="sxs-lookup"><span data-stu-id="ebf37-107">Method</span></span>|<span data-ttu-id="ebf37-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ebf37-108">Return type</span></span>|<span data-ttu-id="ebf37-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebf37-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebf37-110">Listar userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="ebf37-110">List userConsentRequests</span></span>](../api/userconsentrequest-list.md)|<span data-ttu-id="ebf37-111">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="ebf37-111">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="ebf37-112">Obter uma lista dos [objetos userConsentRequest](../resources/userconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ebf37-112">Get a list of the [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="ebf37-113">Obter userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="ebf37-113">Get userConsentRequest</span></span>](../api/userconsentrequest-get.md)|[<span data-ttu-id="ebf37-114">userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="ebf37-114">userConsentRequest</span></span>](../resources/userconsentrequest.md)|<span data-ttu-id="ebf37-115">Leia as propriedades e as relações de um [objeto userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="ebf37-115">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="ebf37-116">Listar userConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="ebf37-116">List userConsentRequests: filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md)|<span data-ttu-id="ebf37-117">[Coleção userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="ebf37-117">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="ebf37-118">Obter uma lista dos [objetos userConsentRequest](../resources/userconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ebf37-118">Get a list of the [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebf37-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebf37-119">Properties</span></span>
|<span data-ttu-id="ebf37-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebf37-120">Property</span></span>|<span data-ttu-id="ebf37-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebf37-121">Type</span></span>|<span data-ttu-id="ebf37-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebf37-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf37-123">approvalId</span><span class="sxs-lookup"><span data-stu-id="ebf37-123">approvalId</span></span>|<span data-ttu-id="ebf37-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebf37-124">String</span></span>|<span data-ttu-id="ebf37-125">A id da aprovação.</span><span class="sxs-lookup"><span data-stu-id="ebf37-125">The id of the approval.</span></span> <span data-ttu-id="ebf37-126">Esse valor é igual ao valor do `id` .</span><span class="sxs-lookup"><span data-stu-id="ebf37-126">This value is equal to the value of the `id`.</span></span>|
|<span data-ttu-id="ebf37-127">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebf37-127">completedDateTime</span></span>|<span data-ttu-id="ebf37-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebf37-128">DateTimeOffset</span></span>|<span data-ttu-id="ebf37-129">A data e a hora em **que o status** da solicitação foi marcado como `Completed` .</span><span class="sxs-lookup"><span data-stu-id="ebf37-129">The date and time when the **status** of the request was marked as `Completed`.</span></span> <span data-ttu-id="ebf37-130">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ebf37-130">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ebf37-131">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ebf37-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="ebf37-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="ebf37-132">createdBy</span></span>|[<span data-ttu-id="ebf37-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="ebf37-133">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="ebf37-134">O usuário que criou a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebf37-134">The user who created the request.</span></span>|
|<span data-ttu-id="ebf37-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebf37-135">createdDateTime</span></span>|<span data-ttu-id="ebf37-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebf37-136">DateTimeOffset</span></span>|<span data-ttu-id="ebf37-137">A data e a hora em que a solicitação foi criada.</span><span class="sxs-lookup"><span data-stu-id="ebf37-137">The date and time when the request was created.</span></span> <span data-ttu-id="ebf37-138">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ebf37-138">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ebf37-139">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ebf37-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="ebf37-140">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="ebf37-140">Supports `$filter` (`eq` only) and `$orderby`.</span></span>|
|<span data-ttu-id="ebf37-141">customData</span><span class="sxs-lookup"><span data-stu-id="ebf37-141">customData</span></span>|<span data-ttu-id="ebf37-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebf37-142">String</span></span>|<span data-ttu-id="ebf37-143">Campo de texto livre para definir quaisquer dados personalizados para a solicitação de consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="ebf37-143">Free text field to define any custom data for the user consent request.</span></span> <span data-ttu-id="ebf37-144">Não usado.</span><span class="sxs-lookup"><span data-stu-id="ebf37-144">Not used.</span></span>|
|<span data-ttu-id="ebf37-145">id</span><span class="sxs-lookup"><span data-stu-id="ebf37-145">id</span></span>|<span data-ttu-id="ebf37-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebf37-146">String</span></span>|<span data-ttu-id="ebf37-147">Identificador da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebf37-147">Identifier of the request.</span></span> |
|<span data-ttu-id="ebf37-148">motivo</span><span class="sxs-lookup"><span data-stu-id="ebf37-148">reason</span></span>|<span data-ttu-id="ebf37-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebf37-149">String</span></span>|<span data-ttu-id="ebf37-150">A justificativa do usuário para exigir acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ebf37-150">The user's justification for requiring access to the app.</span></span> <span data-ttu-id="ebf37-151">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="ebf37-151">Supports `$filter` (`eq` only) and `$orderby`.</span></span>  |
|<span data-ttu-id="ebf37-152">status</span><span class="sxs-lookup"><span data-stu-id="ebf37-152">status</span></span>|<span data-ttu-id="ebf37-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebf37-153">String</span></span>|<span data-ttu-id="ebf37-154">O status da solicitação de consentimento do aplicativo do usuário.</span><span class="sxs-lookup"><span data-stu-id="ebf37-154">The status of the user's app consent request.</span></span> <span data-ttu-id="ebf37-155">Os valores possíveis são: `Initializing` `InProgress` , e `Completed` .</span><span class="sxs-lookup"><span data-stu-id="ebf37-155">Possible values are: `Initializing`, `InProgress`, and `Completed`.</span></span> <span data-ttu-id="ebf37-156">Suporta `$filter` ( `eq` somente) e `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="ebf37-156">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ebf37-157">Relações</span><span class="sxs-lookup"><span data-stu-id="ebf37-157">Relationships</span></span>
|<span data-ttu-id="ebf37-158">Relação</span><span class="sxs-lookup"><span data-stu-id="ebf37-158">Relationship</span></span>|<span data-ttu-id="ebf37-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebf37-159">Type</span></span>|<span data-ttu-id="ebf37-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebf37-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf37-161">aprovação</span><span class="sxs-lookup"><span data-stu-id="ebf37-161">approval</span></span>|[<span data-ttu-id="ebf37-162">aprovação</span><span class="sxs-lookup"><span data-stu-id="ebf37-162">approval</span></span>](../resources/approval.md)|<span data-ttu-id="ebf37-163">Decisões de aprovação associadas a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebf37-163">Approval decisions associated with a request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebf37-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebf37-164">JSON representation</span></span>
<span data-ttu-id="ebf37-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebf37-165">The following is a JSON representation of the resource.</span></span>
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

