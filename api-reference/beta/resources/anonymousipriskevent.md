---
title: tipo de recurso anonymousIpRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory em que uma entrada de conta é tentada a partir de um endereço IP que parece ser anônimo. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5016aac704feb35383dc34e58f3ed06657733edf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013385"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="4cd98-104">tipo de recurso anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4cd98-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cd98-105">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) em que uma entrada de conta é tentada a partir de um endereço IP que parece ser anônimo.</span><span class="sxs-lookup"><span data-stu-id="4cd98-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="4cd98-106">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="4cd98-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="4cd98-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4cd98-107">Methods</span></span>

| <span data-ttu-id="4cd98-108">Método</span><span class="sxs-lookup"><span data-stu-id="4cd98-108">Method</span></span>           | <span data-ttu-id="4cd98-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4cd98-109">Return Type</span></span>    |<span data-ttu-id="4cd98-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cd98-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4cd98-111">Obter anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4cd98-111">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="4cd98-112">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4cd98-112">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="4cd98-113">Leia as propriedades e os relacionamentos do objeto anonymousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="4cd98-113">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4cd98-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cd98-114">Properties</span></span>
| <span data-ttu-id="4cd98-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cd98-115">Property</span></span>     | <span data-ttu-id="4cd98-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cd98-116">Type</span></span>   |<span data-ttu-id="4cd98-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cd98-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cd98-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cd98-118">closedDateTime</span></span>|<span data-ttu-id="4cd98-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cd98-119">dateTimeOffset</span></span>| <span data-ttu-id="4cd98-120">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="4cd98-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="4cd98-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cd98-121">createdDateTime</span></span>|<span data-ttu-id="4cd98-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cd98-122">dateTimeOffset</span></span>| <span data-ttu-id="4cd98-123">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="4cd98-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="4cd98-124">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="4cd98-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="4cd98-125">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="4cd98-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="4cd98-126">id</span><span class="sxs-lookup"><span data-stu-id="4cd98-126">id</span></span>|<span data-ttu-id="4cd98-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cd98-127">string</span></span>| <span data-ttu-id="4cd98-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="4cd98-128">Read-only</span></span>|
|<span data-ttu-id="4cd98-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4cd98-129">ipAddress</span></span>|<span data-ttu-id="4cd98-130">string</span><span class="sxs-lookup"><span data-stu-id="4cd98-130">string</span></span>| <span data-ttu-id="4cd98-131">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="4cd98-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="4cd98-132">location</span><span class="sxs-lookup"><span data-stu-id="4cd98-132">location</span></span>|<span data-ttu-id="4cd98-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cd98-133">string</span></span>| <span data-ttu-id="4cd98-134">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="4cd98-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="4cd98-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="4cd98-135">riskEventDateTime</span></span>|<span data-ttu-id="4cd98-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cd98-136">dateTimeOffset</span></span>| <span data-ttu-id="4cd98-137">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="4cd98-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="4cd98-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="4cd98-138">riskEventStatus</span></span>|<span data-ttu-id="4cd98-139">string</span><span class="sxs-lookup"><span data-stu-id="4cd98-139">string</span></span>| <span data-ttu-id="4cd98-140">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="4cd98-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="4cd98-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="4cd98-141">riskLevel</span></span>|<span data-ttu-id="4cd98-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cd98-142">string</span></span>| <span data-ttu-id="4cd98-143">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4cd98-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="4cd98-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="4cd98-144">riskEventType</span></span>|<span data-ttu-id="4cd98-145">string</span><span class="sxs-lookup"><span data-stu-id="4cd98-145">string</span></span>| <span data-ttu-id="4cd98-146">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="4cd98-146">The type of risk</span></span>|
|<span data-ttu-id="4cd98-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4cd98-147">userDisplayName</span></span>|<span data-ttu-id="4cd98-148">string</span><span class="sxs-lookup"><span data-stu-id="4cd98-148">string</span></span>| <span data-ttu-id="4cd98-149">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="4cd98-149">The name of the user at risk</span></span>|
|<span data-ttu-id="4cd98-150">userId</span><span class="sxs-lookup"><span data-stu-id="4cd98-150">userId</span></span>|<span data-ttu-id="4cd98-151">string</span><span class="sxs-lookup"><span data-stu-id="4cd98-151">string</span></span>| <span data-ttu-id="4cd98-152">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="4cd98-152">The id of the user at risk</span></span>|
|<span data-ttu-id="4cd98-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4cd98-153">userPrincipalName</span></span>|<span data-ttu-id="4cd98-154">string</span><span class="sxs-lookup"><span data-stu-id="4cd98-154">string</span></span>| <span data-ttu-id="4cd98-155">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="4cd98-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cd98-156">Relações</span><span class="sxs-lookup"><span data-stu-id="4cd98-156">Relationships</span></span>
| <span data-ttu-id="4cd98-157">Relação</span><span class="sxs-lookup"><span data-stu-id="4cd98-157">Relationship</span></span> | <span data-ttu-id="4cd98-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cd98-158">Type</span></span>   |<span data-ttu-id="4cd98-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cd98-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cd98-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="4cd98-160">impactedUser</span></span>|[<span data-ttu-id="4cd98-161">Usuário</span><span class="sxs-lookup"><span data-stu-id="4cd98-161">user</span></span>](user.md)| <span data-ttu-id="4cd98-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="4cd98-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cd98-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cd98-164">JSON representation</span></span>

<span data-ttu-id="4cd98-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cd98-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
