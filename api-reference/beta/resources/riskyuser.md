---
title: tipo de recurso de riskyUsers
description: Representa os usuários do Windows Azure AD que estão em risco. Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.
ms.openlocfilehash: 5d51c303d25a781f8e432badb42acb48cf135217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034964"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="3086e-105">tipo de recurso de riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3086e-105">riskyUsers resource type</span></span>

> <span data-ttu-id="3086e-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3086e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3086e-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3086e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3086e-108">Representa os usuários do Windows Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="3086e-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="3086e-109">Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="3086e-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="3086e-110">Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3086e-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="3086e-111">Para obter mais informações sobre eventos de risco, consulte [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="3086e-111">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="3086e-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="3086e-112">Methods</span></span>

| <span data-ttu-id="3086e-113">Método</span><span class="sxs-lookup"><span data-stu-id="3086e-113">Method</span></span>   | <span data-ttu-id="3086e-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3086e-114">Return Type</span></span>|<span data-ttu-id="3086e-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="3086e-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3086e-116">Lista riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3086e-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="3086e-117">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3086e-117">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="3086e-118">Listar usuários riscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3086e-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="3086e-119">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3086e-119">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="3086e-120">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3086e-120">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="3086e-121">Obtenha um usuário riscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3086e-121">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="3086e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3086e-122">Properties</span></span>

| <span data-ttu-id="3086e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3086e-123">Property</span></span>   | <span data-ttu-id="3086e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3086e-124">Type</span></span>|<span data-ttu-id="3086e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3086e-125">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="3086e-126">Id exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="3086e-126">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="3086e-127">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="3086e-127">Indicates whether the user is deleted.</span></span> <span data-ttu-id="3086e-128">Os valores possíveis são: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="3086e-128">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="3086e-129">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="3086e-129">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="3086e-130">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="3086e-130">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="3086e-131">True se a identidade do usuário encontra-se fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="3086e-131">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="3086e-132">Esse usuário pode ser uma B2B ou um usuário B2C com identidade no Azure AD, MSA ou 3º provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="3086e-132">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="3086e-133">False se a identidade do usuário estiver dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="3086e-133">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="3086e-134">Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="3086e-134">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3086e-135">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3086e-135">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="3086e-136">O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.</span><span class="sxs-lookup"><span data-stu-id="3086e-136">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="3086e-137">Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="3086e-137">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3086e-138">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3086e-138">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="3086e-139">O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3086e-139">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="3086e-140">Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="3086e-140">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3086e-141">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3086e-141">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="3086e-142">A data e hora em que o usuário riscado foi atualizada pela última vez</span><span class="sxs-lookup"><span data-stu-id="3086e-142">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="3086e-143">Nome de exibição do usuário riscado</span><span class="sxs-lookup"><span data-stu-id="3086e-143">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="3086e-144">Nome principal de usuário riscado</span><span class="sxs-lookup"><span data-stu-id="3086e-144">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="3086e-145">Relações</span><span class="sxs-lookup"><span data-stu-id="3086e-145">Relationships</span></span>

| <span data-ttu-id="3086e-146">Relação</span><span class="sxs-lookup"><span data-stu-id="3086e-146">Relationship</span></span> | <span data-ttu-id="3086e-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="3086e-147">Type</span></span> |<span data-ttu-id="3086e-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="3086e-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3086e-149">id</span><span class="sxs-lookup"><span data-stu-id="3086e-149">id</span></span>|<span data-ttu-id="3086e-150">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="3086e-150">UserObjectId</span></span>| <span data-ttu-id="3086e-151">O identificador exclusivo do usuário com a qual um evento de determinado risco está associado.</span><span class="sxs-lookup"><span data-stu-id="3086e-151">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="3086e-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="3086e-152">isGuest</span></span>|<span data-ttu-id="3086e-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="3086e-153">isGuest</span></span>| <span data-ttu-id="3086e-154">Um usuário riscado poderia ser um usuário Home (B2E) ou um usuário convidado (B2B, B2C).</span><span class="sxs-lookup"><span data-stu-id="3086e-154">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="3086e-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3086e-155">isDeleted</span></span>|<span data-ttu-id="3086e-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3086e-156">isDeleted</span></span>| <span data-ttu-id="3086e-157">Um usuário pode ou não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="3086e-157">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="3086e-158">riskState</span><span class="sxs-lookup"><span data-stu-id="3086e-158">riskState</span></span>|<span data-ttu-id="3086e-159">riskState</span><span class="sxs-lookup"><span data-stu-id="3086e-159">riskState</span></span>| <span data-ttu-id="3086e-160">Um usuário riscado pode existir em um dos vários estados.</span><span class="sxs-lookup"><span data-stu-id="3086e-160">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="3086e-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3086e-161">riskDetail</span></span>|<span data-ttu-id="3086e-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3086e-162">riskDetail</span></span>| <span data-ttu-id="3086e-163">Um usuário riscado poderia ser em um determinado estado por vários motivos.</span><span class="sxs-lookup"><span data-stu-id="3086e-163">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="3086e-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3086e-164">riskLevel</span></span>|<span data-ttu-id="3086e-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3086e-165">riskLevel</span></span>| <span data-ttu-id="3086e-166">Um usuário riscado poderia ser considerado um dos vários níveis de risco.</span><span class="sxs-lookup"><span data-stu-id="3086e-166">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3086e-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3086e-167">JSON representation</span></span>

<span data-ttu-id="3086e-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3086e-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"}
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
