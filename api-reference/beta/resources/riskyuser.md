---
title: tipo de recurso riskyUser
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3548be0439eaa5335d710a35f51fdbaecb19060c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008723"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="8af4d-105">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="8af4d-105">riskyUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8af4d-106">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="8af4d-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="8af4d-107">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="8af4d-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="8af4d-108">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8af4d-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="8af4d-109">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="8af4d-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="8af4d-110">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="8af4d-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="8af4d-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="8af4d-111">Methods</span></span>

| <span data-ttu-id="8af4d-112">Método</span><span class="sxs-lookup"><span data-stu-id="8af4d-112">Method</span></span>   | <span data-ttu-id="8af4d-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8af4d-113">Return Type</span></span>|<span data-ttu-id="8af4d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="8af4d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8af4d-115">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="8af4d-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="8af4d-116">coleção [riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="8af4d-116">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="8af4d-117">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8af4d-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="8af4d-118">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="8af4d-118">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="8af4d-119">riskyUser</span><span class="sxs-lookup"><span data-stu-id="8af4d-119">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="8af4d-120">Obtenha um usuário arriscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8af4d-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="8af4d-121">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="8af4d-121">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="8af4d-122">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8af4d-122">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="8af4d-123">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8af4d-123">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="8af4d-124">Confirmar riskyUsers comprometido</span><span class="sxs-lookup"><span data-stu-id="8af4d-124">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="8af4d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8af4d-125">None</span></span> |<span data-ttu-id="8af4d-126">Confirmar um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="8af4d-126">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="8af4d-127">Ignorar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="8af4d-127">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="8af4d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8af4d-128">None</span></span> | <span data-ttu-id="8af4d-129">Descartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="8af4d-129">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="8af4d-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8af4d-130">Properties</span></span>

| <span data-ttu-id="8af4d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8af4d-131">Property</span></span>   | <span data-ttu-id="8af4d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8af4d-132">Type</span></span>|<span data-ttu-id="8af4d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8af4d-133">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="8af4d-134">ID exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="8af4d-134">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="8af4d-135">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="8af4d-135">Indicates whether the user is deleted.</span></span> <span data-ttu-id="8af4d-136">Os valores possíveis são `true`:,`false`</span><span class="sxs-lookup"><span data-stu-id="8af4d-136">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="8af4d-137">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="8af4d-137">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="8af4d-138">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="8af4d-138">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="8af4d-139">True se a identidade do usuário está fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="8af4d-139">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="8af4d-140">Este usuário pode ser um usuário B2B ou B2C com identidade no Azure AD, no MSA ou no provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="8af4d-140">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="8af4d-141">False se a identidade do usuário está dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="8af4d-141">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="8af4d-142">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="8af4d-142">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="8af4d-143">A data e a hora em que o usuário arriscado foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="8af4d-143">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="8af4d-144">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="8af4d-144">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="8af4d-145">Os valores possíveis são None, confirmedSafe, remediated, atRisk, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="8af4d-145">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="8af4d-146">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="8af4d-146">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="8af4d-147">Nome de exibição do usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="8af4d-147">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="8af4d-148">Nome UPN de usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="8af4d-148">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="8af4d-149">Relações</span><span class="sxs-lookup"><span data-stu-id="8af4d-149">Relationships</span></span>
| <span data-ttu-id="8af4d-150">Relação</span><span class="sxs-lookup"><span data-stu-id="8af4d-150">Relationship</span></span> | <span data-ttu-id="8af4d-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="8af4d-151">Type</span></span>   |<span data-ttu-id="8af4d-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="8af4d-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8af4d-153">histórico</span><span class="sxs-lookup"><span data-stu-id="8af4d-153">history</span></span>|<span data-ttu-id="8af4d-154">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8af4d-154">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="8af4d-155">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8af4d-155">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8af4d-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8af4d-156">JSON representation</span></span>

<span data-ttu-id="8af4d-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8af4d-157">Here is a JSON representation of the resource.</span></span>

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
