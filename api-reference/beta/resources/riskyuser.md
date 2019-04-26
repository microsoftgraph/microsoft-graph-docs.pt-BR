---
title: tipo de recurso riskyUser
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179a6cbddf3e4b27c47761bd81aad1052ae7f728
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343532"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="7d76d-105">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="7d76d-105">riskyUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d76d-106">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="7d76d-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="7d76d-107">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="7d76d-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="7d76d-108">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7d76d-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="7d76d-109">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="7d76d-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="7d76d-110">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="7d76d-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="7d76d-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d76d-111">Methods</span></span>

| <span data-ttu-id="7d76d-112">Método</span><span class="sxs-lookup"><span data-stu-id="7d76d-112">Method</span></span>   | <span data-ttu-id="7d76d-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d76d-113">Return Type</span></span>|<span data-ttu-id="7d76d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d76d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d76d-115">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7d76d-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="7d76d-116">coleção [riskyUser](riskyUser.md)</span><span class="sxs-lookup"><span data-stu-id="7d76d-116">[riskyUser](riskyUser.md) collection</span></span>|<span data-ttu-id="7d76d-117">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="7d76d-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="7d76d-118">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="7d76d-118">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="7d76d-119">riskyUser</span><span class="sxs-lookup"><span data-stu-id="7d76d-119">riskyUser</span></span>](riskyUser.md)|<span data-ttu-id="7d76d-120">Obtenha um usuário arriscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="7d76d-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="7d76d-121">Confirmar riskyUsers comprometido</span><span class="sxs-lookup"><span data-stu-id="7d76d-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="7d76d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d76d-122">None</span></span> |<span data-ttu-id="7d76d-123">Confirmar um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="7d76d-123">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="7d76d-124">Ignorar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7d76d-124">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="7d76d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d76d-125">None</span></span> | <span data-ttu-id="7d76d-126">DesCartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="7d76d-126">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d76d-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d76d-127">Properties</span></span>

| <span data-ttu-id="7d76d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d76d-128">Property</span></span>   | <span data-ttu-id="7d76d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d76d-129">Type</span></span>|<span data-ttu-id="7d76d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d76d-130">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="7d76d-131">ID exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="7d76d-131">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="7d76d-132">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="7d76d-132">Indicates whether the user is deleted.</span></span> <span data-ttu-id="7d76d-133">Os valores possíveis são `true`:,`false`</span><span class="sxs-lookup"><span data-stu-id="7d76d-133">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="7d76d-134">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="7d76d-134">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="7d76d-135">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="7d76d-135">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="7d76d-136">True se a identidade do usuário está fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="7d76d-136">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="7d76d-137">Este usuário pode ser um usuário B2B ou B2C com identidade no Azure AD, no MSA ou no provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="7d76d-137">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="7d76d-138">False se a identidade do usuário está dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="7d76d-138">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="7d76d-139">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="7d76d-139">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="7d76d-140">A data e a hora em que o usuário arriscado foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="7d76d-140">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="7d76d-141">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="7d76d-141">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="7d76d-142">Os valores possíveis são None, confirmedSafe, remediated, atRisk, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="7d76d-142">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="7d76d-143">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="7d76d-143">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="7d76d-144">Nome de exibição do usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="7d76d-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="7d76d-145">Nome UPN de usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="7d76d-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d76d-146">Relações</span><span class="sxs-lookup"><span data-stu-id="7d76d-146">Relationships</span></span>
| <span data-ttu-id="7d76d-147">Relação</span><span class="sxs-lookup"><span data-stu-id="7d76d-147">Relationship</span></span> | <span data-ttu-id="7d76d-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d76d-148">Type</span></span>   |<span data-ttu-id="7d76d-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d76d-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d76d-150">histórico</span><span class="sxs-lookup"><span data-stu-id="7d76d-150">history</span></span>|<span data-ttu-id="7d76d-151">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7d76d-151">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>| |

## <a name="json-representation"></a><span data-ttu-id="7d76d-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d76d-152">JSON representation</span></span>

<span data-ttu-id="7d76d-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d76d-153">Here is a JSON representation of the resource.</span></span>

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
