---
title: tipo de recurso leakedCredentialsRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde as credenciais de uma conta foram detectadas. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
ms.openlocfilehash: 1fbba14c25678b0e847c18648970a9fb551bee48
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345327"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="c2ab7-104">tipo de recurso leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c2ab7-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2ab7-105">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde as credenciais de uma conta foram detectadas.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="c2ab7-106">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="c2ab7-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="c2ab7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c2ab7-107">Methods</span></span>

| <span data-ttu-id="c2ab7-108">Método</span><span class="sxs-lookup"><span data-stu-id="c2ab7-108">Method</span></span>           | <span data-ttu-id="c2ab7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c2ab7-109">Return Type</span></span>    |<span data-ttu-id="c2ab7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ab7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2ab7-111">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c2ab7-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="c2ab7-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c2ab7-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="c2ab7-113">Leia as propriedades e os relacionamentos do objeto leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2ab7-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2ab7-114">Properties</span></span>
| <span data-ttu-id="c2ab7-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2ab7-115">Property</span></span>     | <span data-ttu-id="c2ab7-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2ab7-116">Type</span></span>   |<span data-ttu-id="c2ab7-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ab7-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2ab7-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2ab7-118">closedDateTime</span></span>|<span data-ttu-id="c2ab7-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2ab7-119">dateTimeOffset</span></span>| <span data-ttu-id="c2ab7-120">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="c2ab7-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c2ab7-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2ab7-121">createdDateTime</span></span>|<span data-ttu-id="c2ab7-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2ab7-122">dateTimeOffset</span></span>| <span data-ttu-id="c2ab7-123">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="c2ab7-124">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c2ab7-125">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c2ab7-126">id</span><span class="sxs-lookup"><span data-stu-id="c2ab7-126">id</span></span>|<span data-ttu-id="c2ab7-127">string</span><span class="sxs-lookup"><span data-stu-id="c2ab7-127">string</span></span>| <span data-ttu-id="c2ab7-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c2ab7-128">Read-only</span></span>|
|<span data-ttu-id="c2ab7-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c2ab7-129">riskEventDateTime</span></span>|<span data-ttu-id="c2ab7-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2ab7-130">dateTimeOffset</span></span>| <span data-ttu-id="c2ab7-131">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="c2ab7-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c2ab7-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c2ab7-132">riskEventStatus</span></span>|<span data-ttu-id="c2ab7-133">string</span><span class="sxs-lookup"><span data-stu-id="c2ab7-133">string</span></span>| <span data-ttu-id="c2ab7-134">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c2ab7-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c2ab7-135">riskLevel</span></span>|<span data-ttu-id="c2ab7-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2ab7-136">string</span></span>| <span data-ttu-id="c2ab7-137">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c2ab7-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c2ab7-138">riskEventType</span></span>|<span data-ttu-id="c2ab7-139">string</span><span class="sxs-lookup"><span data-stu-id="c2ab7-139">string</span></span>| <span data-ttu-id="c2ab7-140">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="c2ab7-140">The type of risk</span></span>|
|<span data-ttu-id="c2ab7-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2ab7-141">userDisplayName</span></span>|<span data-ttu-id="c2ab7-142">string</span><span class="sxs-lookup"><span data-stu-id="c2ab7-142">string</span></span>| <span data-ttu-id="c2ab7-143">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c2ab7-143">The name of the user at risk</span></span>|
|<span data-ttu-id="c2ab7-144">userId</span><span class="sxs-lookup"><span data-stu-id="c2ab7-144">userId</span></span>|<span data-ttu-id="c2ab7-145">string</span><span class="sxs-lookup"><span data-stu-id="c2ab7-145">string</span></span>| <span data-ttu-id="c2ab7-146">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c2ab7-146">The id of the user at risk</span></span>|
|<span data-ttu-id="c2ab7-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2ab7-147">userPrincipalName</span></span>|<span data-ttu-id="c2ab7-148">string</span><span class="sxs-lookup"><span data-stu-id="c2ab7-148">string</span></span>| <span data-ttu-id="c2ab7-149">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c2ab7-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2ab7-150">Relações</span><span class="sxs-lookup"><span data-stu-id="c2ab7-150">Relationships</span></span>
| <span data-ttu-id="c2ab7-151">Relação</span><span class="sxs-lookup"><span data-stu-id="c2ab7-151">Relationship</span></span> | <span data-ttu-id="c2ab7-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2ab7-152">Type</span></span>   |<span data-ttu-id="c2ab7-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ab7-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2ab7-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c2ab7-154">impactedUser</span></span>|[<span data-ttu-id="c2ab7-155">user</span><span class="sxs-lookup"><span data-stu-id="c2ab7-155">user</span></span>](user.md)| <span data-ttu-id="c2ab7-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2ab7-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2ab7-158">JSON representation</span></span>

<span data-ttu-id="c2ab7-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2ab7-159">Here is a JSON representation of the resource.</span></span>

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
