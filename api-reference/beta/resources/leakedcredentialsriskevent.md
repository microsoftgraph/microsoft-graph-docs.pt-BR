---
title: Tipo de recurso leakedCredentialsRiskEvent
description: Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory onde as credenciais de uma conta foram detectadas na natureza. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: ac8e9dc0c2adb685513c74658464f4a79af5cb45
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442975"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a><span data-ttu-id="218c8-104">Tipo de recurso leakedCredentialsRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="218c8-104">leakedCredentialsRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="218c8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="218c8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="218c8-106">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="218c8-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="218c8-107">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="218c8-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="218c8-108">Um evento de risco detectado pela Proteção de Identidade do [Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde as credenciais de uma conta foram detectadas na natureza.</span><span class="sxs-lookup"><span data-stu-id="218c8-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="218c8-109">Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="218c8-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="218c8-110">Methods</span><span class="sxs-lookup"><span data-stu-id="218c8-110">Methods</span></span>

| <span data-ttu-id="218c8-111">Método</span><span class="sxs-lookup"><span data-stu-id="218c8-111">Method</span></span>           | <span data-ttu-id="218c8-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="218c8-112">Return Type</span></span>    |<span data-ttu-id="218c8-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="218c8-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="218c8-114">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="218c8-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="218c8-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="218c8-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="218c8-116">Leia propriedades e relações do objeto leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="218c8-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="218c8-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="218c8-117">Properties</span></span>
| <span data-ttu-id="218c8-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="218c8-118">Property</span></span>     | <span data-ttu-id="218c8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="218c8-119">Type</span></span>   |<span data-ttu-id="218c8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="218c8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="218c8-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="218c8-121">closedDateTime</span></span>|<span data-ttu-id="218c8-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="218c8-122">dateTimeOffset</span></span>| <span data-ttu-id="218c8-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="218c8-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="218c8-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="218c8-124">createdDateTime</span></span>|<span data-ttu-id="218c8-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="218c8-125">dateTimeOffset</span></span>| <span data-ttu-id="218c8-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="218c8-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="218c8-127">Isso é sempre maior ou igual ao tempo de data do evento de risco em si.</span><span class="sxs-lookup"><span data-stu-id="218c8-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="218c8-128">Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="218c8-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="218c8-129">id</span><span class="sxs-lookup"><span data-stu-id="218c8-129">id</span></span>|<span data-ttu-id="218c8-130">string</span><span class="sxs-lookup"><span data-stu-id="218c8-130">string</span></span>| <span data-ttu-id="218c8-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="218c8-131">Read-only</span></span>|
|<span data-ttu-id="218c8-132">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="218c8-132">riskEventDateTime</span></span>|<span data-ttu-id="218c8-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="218c8-133">dateTimeOffset</span></span>| <span data-ttu-id="218c8-134">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="218c8-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="218c8-135">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="218c8-135">riskEventStatus</span></span>|<span data-ttu-id="218c8-136">string</span><span class="sxs-lookup"><span data-stu-id="218c8-136">string</span></span>| <span data-ttu-id="218c8-137">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="218c8-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="218c8-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="218c8-138">riskLevel</span></span>|<span data-ttu-id="218c8-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="218c8-139">string</span></span>| <span data-ttu-id="218c8-140">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="218c8-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="218c8-141">riskEventType</span><span class="sxs-lookup"><span data-stu-id="218c8-141">riskEventType</span></span>|<span data-ttu-id="218c8-142">string</span><span class="sxs-lookup"><span data-stu-id="218c8-142">string</span></span>| <span data-ttu-id="218c8-143">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="218c8-143">The type of risk</span></span>|
|<span data-ttu-id="218c8-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="218c8-144">userDisplayName</span></span>|<span data-ttu-id="218c8-145">string</span><span class="sxs-lookup"><span data-stu-id="218c8-145">string</span></span>| <span data-ttu-id="218c8-146">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="218c8-146">The name of the user at risk</span></span>|
|<span data-ttu-id="218c8-147">userId</span><span class="sxs-lookup"><span data-stu-id="218c8-147">userId</span></span>|<span data-ttu-id="218c8-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="218c8-148">string</span></span>| <span data-ttu-id="218c8-149">A id do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="218c8-149">The id of the user at risk</span></span>|
|<span data-ttu-id="218c8-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="218c8-150">userPrincipalName</span></span>|<span data-ttu-id="218c8-151">string</span><span class="sxs-lookup"><span data-stu-id="218c8-151">string</span></span>| <span data-ttu-id="218c8-152">O nome principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="218c8-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="218c8-153">Relações</span><span class="sxs-lookup"><span data-stu-id="218c8-153">Relationships</span></span>
| <span data-ttu-id="218c8-154">Relação</span><span class="sxs-lookup"><span data-stu-id="218c8-154">Relationship</span></span> | <span data-ttu-id="218c8-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="218c8-155">Type</span></span>   |<span data-ttu-id="218c8-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="218c8-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="218c8-157">impactedUser</span><span class="sxs-lookup"><span data-stu-id="218c8-157">impactedUser</span></span>|[<span data-ttu-id="218c8-158">user</span><span class="sxs-lookup"><span data-stu-id="218c8-158">user</span></span>](user.md)| <span data-ttu-id="218c8-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="218c8-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="218c8-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="218c8-161">JSON representation</span></span>

<span data-ttu-id="218c8-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="218c8-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
