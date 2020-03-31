---
title: tipo de recurso riskyUser
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7759a9c42ca9178dc95266ffa4630ef891832ecd
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062634"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="407a2-105">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="407a2-105">riskyUser resource type</span></span>

<span data-ttu-id="407a2-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="407a2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="407a2-107">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="407a2-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="407a2-108">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="407a2-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="407a2-109">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="407a2-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="407a2-110">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="407a2-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="407a2-111">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="407a2-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="407a2-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="407a2-112">Methods</span></span>

| <span data-ttu-id="407a2-113">Método</span><span class="sxs-lookup"><span data-stu-id="407a2-113">Method</span></span>   | <span data-ttu-id="407a2-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="407a2-114">Return Type</span></span>|<span data-ttu-id="407a2-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="407a2-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="407a2-116">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="407a2-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="407a2-117">coleção [riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="407a2-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="407a2-118">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="407a2-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="407a2-119">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="407a2-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="407a2-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="407a2-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="407a2-121">Obtenha um usuário arriscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="407a2-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="407a2-122">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="407a2-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="407a2-123">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="407a2-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="407a2-124">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="407a2-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="407a2-125">Confirmar riskyUsers comprometido</span><span class="sxs-lookup"><span data-stu-id="407a2-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="407a2-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="407a2-126">None</span></span> |<span data-ttu-id="407a2-127">Confirmar um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="407a2-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="407a2-128">Ignorar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="407a2-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="407a2-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="407a2-129">None</span></span> | <span data-ttu-id="407a2-130">Descartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="407a2-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="407a2-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="407a2-131">Properties</span></span>

| <span data-ttu-id="407a2-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="407a2-132">Property</span></span>   | <span data-ttu-id="407a2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="407a2-133">Type</span></span>|<span data-ttu-id="407a2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="407a2-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="407a2-135">ID exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="407a2-135">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="407a2-136">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="407a2-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="407a2-137">Os valores possíveis são `true`:,`false`</span><span class="sxs-lookup"><span data-stu-id="407a2-137">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="407a2-138">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="407a2-138">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="407a2-139">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="407a2-139">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="407a2-140">True se a identidade do usuário está fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="407a2-140">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="407a2-141">Este usuário pode ser um usuário B2B ou B2C com identidade no Azure AD, no MSA ou no provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="407a2-141">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="407a2-142">False se a identidade do usuário está dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="407a2-142">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="407a2-143">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="407a2-143">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="407a2-144">A data e a hora em que o usuário arriscado foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="407a2-144">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="407a2-145">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="407a2-145">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="407a2-146">Os valores possíveis são None, confirmedSafe, remediated, atRisk, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="407a2-146">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="407a2-147">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="407a2-147">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="407a2-148">Nome de exibição do usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="407a2-148">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="407a2-149">Nome UPN de usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="407a2-149">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="407a2-150">Relações</span><span class="sxs-lookup"><span data-stu-id="407a2-150">Relationships</span></span>

<span data-ttu-id="407a2-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="407a2-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="407a2-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="407a2-152">JSON representation</span></span>

<span data-ttu-id="407a2-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="407a2-153">The following is a JSON representation of the resource.</span></span>

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
"isGuest": "boolean",
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
