---
title: tipo de recurso de riskyUsers
description: Representa os usuários do Windows Azure AD que estão em risco. Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: bb1dab6461a3b235d461720a68855f1e8f3f70d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871551"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="3bcfe-105">tipo de recurso de riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3bcfe-105">riskyUsers resource type</span></span>

> <span data-ttu-id="3bcfe-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bcfe-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3bcfe-108">Representa os usuários do Windows Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="3bcfe-109">Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="3bcfe-110">Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="3bcfe-111">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="3bcfe-112">Para obter mais informações sobre eventos de risco, consulte [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="3bcfe-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="3bcfe-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="3bcfe-113">Methods</span></span>

| <span data-ttu-id="3bcfe-114">Método</span><span class="sxs-lookup"><span data-stu-id="3bcfe-114">Method</span></span>   | <span data-ttu-id="3bcfe-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3bcfe-115">Return Type</span></span>|<span data-ttu-id="3bcfe-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bcfe-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3bcfe-117">Lista riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3bcfe-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="3bcfe-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3bcfe-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="3bcfe-119">Listar usuários riscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="3bcfe-120">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3bcfe-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="3bcfe-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3bcfe-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="3bcfe-122">Obtenha um usuário riscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="3bcfe-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bcfe-123">Properties</span></span>

| <span data-ttu-id="3bcfe-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bcfe-124">Property</span></span>   | <span data-ttu-id="3bcfe-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bcfe-125">Type</span></span>|<span data-ttu-id="3bcfe-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bcfe-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="3bcfe-127">Id exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="3bcfe-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="3bcfe-128">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="3bcfe-129">Os valores possíveis são: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="3bcfe-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="3bcfe-130">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="3bcfe-131">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="3bcfe-132">True se a identidade do usuário encontra-se fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="3bcfe-133">Esse usuário pode ser uma B2B ou um usuário B2C com identidade no Azure AD, MSA ou 3º provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="3bcfe-134">False se a identidade do usuário estiver dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="3bcfe-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="3bcfe-135">Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3bcfe-136">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="3bcfe-137">O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="3bcfe-138">Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3bcfe-139">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="3bcfe-140">O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="3bcfe-141">Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3bcfe-142">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="3bcfe-143">A data e hora em que o usuário riscado foi atualizada pela última vez</span><span class="sxs-lookup"><span data-stu-id="3bcfe-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="3bcfe-144">Nome de exibição do usuário riscado</span><span class="sxs-lookup"><span data-stu-id="3bcfe-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="3bcfe-145">Nome principal de usuário riscado</span><span class="sxs-lookup"><span data-stu-id="3bcfe-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bcfe-146">Relações</span><span class="sxs-lookup"><span data-stu-id="3bcfe-146">Relationships</span></span>

| <span data-ttu-id="3bcfe-147">Relação</span><span class="sxs-lookup"><span data-stu-id="3bcfe-147">Relationship</span></span> | <span data-ttu-id="3bcfe-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bcfe-148">Type</span></span> |<span data-ttu-id="3bcfe-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bcfe-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bcfe-150">id</span><span class="sxs-lookup"><span data-stu-id="3bcfe-150">id</span></span>|<span data-ttu-id="3bcfe-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="3bcfe-151">UserObjectId</span></span>| <span data-ttu-id="3bcfe-152">O identificador exclusivo do usuário com a qual um evento de determinado risco está associado.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="3bcfe-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="3bcfe-153">isGuest</span></span>|<span data-ttu-id="3bcfe-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="3bcfe-154">isGuest</span></span>| <span data-ttu-id="3bcfe-155">Um usuário riscado poderia ser um usuário Home (B2E) ou um usuário convidado (B2B, B2C).</span><span class="sxs-lookup"><span data-stu-id="3bcfe-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="3bcfe-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3bcfe-156">isDeleted</span></span>|<span data-ttu-id="3bcfe-157">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3bcfe-157">isDeleted</span></span>| <span data-ttu-id="3bcfe-158">Um usuário pode ou não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="3bcfe-159">riskState</span><span class="sxs-lookup"><span data-stu-id="3bcfe-159">riskState</span></span>|<span data-ttu-id="3bcfe-160">riskState</span><span class="sxs-lookup"><span data-stu-id="3bcfe-160">riskState</span></span>| <span data-ttu-id="3bcfe-161">Um usuário riscado pode existir em um dos vários estados.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="3bcfe-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3bcfe-162">riskDetail</span></span>|<span data-ttu-id="3bcfe-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3bcfe-163">riskDetail</span></span>| <span data-ttu-id="3bcfe-164">Um usuário riscado poderia ser em um determinado estado por vários motivos.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="3bcfe-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3bcfe-165">riskLevel</span></span>|<span data-ttu-id="3bcfe-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3bcfe-166">riskLevel</span></span>| <span data-ttu-id="3bcfe-167">Um usuário riscado poderia ser considerado um dos vários níveis de risco.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3bcfe-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bcfe-168">JSON representation</span></span>

<span data-ttu-id="3bcfe-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bcfe-169">Here is a JSON representation of the resource.</span></span>

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
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
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
