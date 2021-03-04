---
title: tipo de recurso riskyUser
description: Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9a234bc4c84ed6acc569f98c8c9b5d475a5b56be
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442850"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="e5955-105">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="e5955-105">riskyUser resource type</span></span>

<span data-ttu-id="e5955-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5955-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5955-107">Representa os usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="e5955-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="e5955-108">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="e5955-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="e5955-109">Essa API fornece acesso programático a todos os usuários em risco no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5955-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="e5955-110">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="e5955-110">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="e5955-111">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="e5955-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="e5955-112">Methods</span><span class="sxs-lookup"><span data-stu-id="e5955-112">Methods</span></span>

| <span data-ttu-id="e5955-113">Método</span><span class="sxs-lookup"><span data-stu-id="e5955-113">Method</span></span>   | <span data-ttu-id="e5955-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e5955-114">Return Type</span></span>|<span data-ttu-id="e5955-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5955-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5955-116">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e5955-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="e5955-117">[Coleção riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5955-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="e5955-118">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e5955-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="e5955-119">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="e5955-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="e5955-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="e5955-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="e5955-121">Obter um usuário de risco específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e5955-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="e5955-122">Histórico de listas</span><span class="sxs-lookup"><span data-stu-id="e5955-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="e5955-123">[coleção riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5955-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="e5955-124">Obter o histórico de risco de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5955-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="e5955-125">Confirmar riskyUsers comprometidos</span><span class="sxs-lookup"><span data-stu-id="e5955-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="e5955-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="e5955-126">None</span></span> |<span data-ttu-id="e5955-127">Confirme um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="e5955-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="e5955-128">Descartar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e5955-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="e5955-129">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="e5955-129">None</span></span> | <span data-ttu-id="e5955-130">Descartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="e5955-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5955-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5955-131">Properties</span></span>

| <span data-ttu-id="e5955-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5955-132">Property</span></span>   | <span data-ttu-id="e5955-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5955-133">Type</span></span>|<span data-ttu-id="e5955-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5955-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="e5955-135">ID exclusiva do usuário em risco.</span><span class="sxs-lookup"><span data-stu-id="e5955-135">Unique ID of the user at risk.</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="e5955-136">Indica se o usuário foi excluído.</span><span class="sxs-lookup"><span data-stu-id="e5955-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="e5955-137">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="e5955-137">Possible values are: `true`, `false`.</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="e5955-138">Indica se o estado de risco de um usuário está sendo processado pelo back-end.</span><span class="sxs-lookup"><span data-stu-id="e5955-138">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="e5955-139">A data e a hora em que o usuário arriscado foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="e5955-139">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="e5955-140">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="e5955-140">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="e5955-141">Os valores possíveis são none, confirmedSafe, remediado, atRisk, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="e5955-141">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="e5955-142">Os valores possíveis não são nenhum, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="e5955-142">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="e5955-143">Nome de exibição de usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="e5955-143">Risky user display name.</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="e5955-144">Nome principal do usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="e5955-144">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5955-145">Relações</span><span class="sxs-lookup"><span data-stu-id="e5955-145">Relationships</span></span>

<span data-ttu-id="e5955-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5955-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5955-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5955-147">JSON representation</span></span>

<span data-ttu-id="e5955-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5955-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
