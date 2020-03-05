---
title: tipo de recurso riskyUser
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5cb1087323287f3c8e752810b1c37365c8268a19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521058"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="70e6d-105">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="70e6d-105">riskyUser resource type</span></span>

<span data-ttu-id="70e6d-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="70e6d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70e6d-107">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="70e6d-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="70e6d-108">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="70e6d-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="70e6d-109">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70e6d-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="70e6d-110">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="70e6d-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="70e6d-111">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="70e6d-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="70e6d-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="70e6d-112">Methods</span></span>

| <span data-ttu-id="70e6d-113">Método</span><span class="sxs-lookup"><span data-stu-id="70e6d-113">Method</span></span>   | <span data-ttu-id="70e6d-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="70e6d-114">Return Type</span></span>|<span data-ttu-id="70e6d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e6d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70e6d-116">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="70e6d-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="70e6d-117">coleção [riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="70e6d-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="70e6d-118">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="70e6d-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="70e6d-119">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="70e6d-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="70e6d-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="70e6d-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="70e6d-121">Obtenha um usuário arriscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="70e6d-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="70e6d-122">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="70e6d-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="70e6d-123">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="70e6d-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="70e6d-124">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70e6d-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="70e6d-125">Confirmar riskyUsers comprometido</span><span class="sxs-lookup"><span data-stu-id="70e6d-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="70e6d-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70e6d-126">None</span></span> |<span data-ttu-id="70e6d-127">Confirmar um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="70e6d-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="70e6d-128">Ignorar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="70e6d-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="70e6d-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70e6d-129">None</span></span> | <span data-ttu-id="70e6d-130">Descartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="70e6d-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="70e6d-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70e6d-131">Properties</span></span>

| <span data-ttu-id="70e6d-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70e6d-132">Property</span></span>   | <span data-ttu-id="70e6d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="70e6d-133">Type</span></span>|<span data-ttu-id="70e6d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e6d-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="70e6d-135">ID exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="70e6d-135">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="70e6d-136">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="70e6d-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="70e6d-137">Os valores possíveis são `true`:,`false`</span><span class="sxs-lookup"><span data-stu-id="70e6d-137">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="70e6d-138">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="70e6d-138">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="70e6d-139">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="70e6d-139">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="70e6d-140">True se a identidade do usuário está fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="70e6d-140">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="70e6d-141">Este usuário pode ser um usuário B2B ou B2C com identidade no Azure AD, no MSA ou no provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="70e6d-141">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="70e6d-142">False se a identidade do usuário está dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="70e6d-142">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="70e6d-143">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="70e6d-143">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="70e6d-144">A data e a hora em que o usuário arriscado foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="70e6d-144">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="70e6d-145">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="70e6d-145">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="70e6d-146">Os valores possíveis são None, confirmedSafe, remediated, atRisk, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="70e6d-146">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="70e6d-147">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="70e6d-147">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="70e6d-148">Nome de exibição do usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="70e6d-148">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="70e6d-149">Nome UPN de usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="70e6d-149">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="70e6d-150">Relações</span><span class="sxs-lookup"><span data-stu-id="70e6d-150">Relationships</span></span>
| <span data-ttu-id="70e6d-151">Relação</span><span class="sxs-lookup"><span data-stu-id="70e6d-151">Relationship</span></span> | <span data-ttu-id="70e6d-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="70e6d-152">Type</span></span>   |<span data-ttu-id="70e6d-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e6d-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70e6d-154">histórico</span><span class="sxs-lookup"><span data-stu-id="70e6d-154">history</span></span>|<span data-ttu-id="70e6d-155">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="70e6d-155">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="70e6d-156">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70e6d-156">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70e6d-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70e6d-157">JSON representation</span></span>

<span data-ttu-id="70e6d-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70e6d-158">Here is a JSON representation of the resource.</span></span>

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
