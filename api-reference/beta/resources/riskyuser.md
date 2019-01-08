---
title: tipo de recurso de riskyUsers
description: Representa os usuários do Windows Azure AD que estão em risco. Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.
author: cloudhandler
ms.openlocfilehash: bc8b64b93662511fffe709a18fb3e7210f3a941b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748259"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="0ed5b-105">tipo de recurso de riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0ed5b-105">riskyUsers resource type</span></span>

> <span data-ttu-id="0ed5b-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ed5b-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ed5b-108">Representa os usuários do Windows Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="0ed5b-109">Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="0ed5b-110">Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="0ed5b-111">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="0ed5b-112">Para obter mais informações sobre eventos de risco, consulte [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="0ed5b-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="0ed5b-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ed5b-113">Methods</span></span>

| <span data-ttu-id="0ed5b-114">Método</span><span class="sxs-lookup"><span data-stu-id="0ed5b-114">Method</span></span>   | <span data-ttu-id="0ed5b-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0ed5b-115">Return Type</span></span>|<span data-ttu-id="0ed5b-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ed5b-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ed5b-117">Lista riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0ed5b-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="0ed5b-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0ed5b-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="0ed5b-119">Listar usuários riscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="0ed5b-120">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0ed5b-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="0ed5b-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0ed5b-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="0ed5b-122">Obtenha um usuário riscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ed5b-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ed5b-123">Properties</span></span>

| <span data-ttu-id="0ed5b-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ed5b-124">Property</span></span>   | <span data-ttu-id="0ed5b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ed5b-125">Type</span></span>|<span data-ttu-id="0ed5b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ed5b-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="0ed5b-127">Id exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="0ed5b-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="0ed5b-128">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="0ed5b-129">Os valores possíveis são: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="0ed5b-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="0ed5b-130">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="0ed5b-131">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="0ed5b-132">True se a identidade do usuário encontra-se fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="0ed5b-133">Esse usuário pode ser uma B2B ou um usuário B2C com identidade no Azure AD, MSA ou 3º provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="0ed5b-134">False se a identidade do usuário estiver dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="0ed5b-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="0ed5b-135">Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="0ed5b-136">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="0ed5b-137">O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="0ed5b-138">Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="0ed5b-139">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="0ed5b-140">O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="0ed5b-141">Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="0ed5b-142">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="0ed5b-143">A data e hora em que o usuário riscado foi atualizada pela última vez</span><span class="sxs-lookup"><span data-stu-id="0ed5b-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="0ed5b-144">Nome de exibição do usuário riscado</span><span class="sxs-lookup"><span data-stu-id="0ed5b-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="0ed5b-145">Nome principal de usuário riscado</span><span class="sxs-lookup"><span data-stu-id="0ed5b-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ed5b-146">Relações</span><span class="sxs-lookup"><span data-stu-id="0ed5b-146">Relationships</span></span>

| <span data-ttu-id="0ed5b-147">Relação</span><span class="sxs-lookup"><span data-stu-id="0ed5b-147">Relationship</span></span> | <span data-ttu-id="0ed5b-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ed5b-148">Type</span></span> |<span data-ttu-id="0ed5b-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ed5b-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ed5b-150">id</span><span class="sxs-lookup"><span data-stu-id="0ed5b-150">id</span></span>|<span data-ttu-id="0ed5b-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="0ed5b-151">UserObjectId</span></span>| <span data-ttu-id="0ed5b-152">O identificador exclusivo do usuário com a qual um evento de determinado risco está associado.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="0ed5b-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="0ed5b-153">isGuest</span></span>|<span data-ttu-id="0ed5b-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="0ed5b-154">isGuest</span></span>| <span data-ttu-id="0ed5b-155">Um usuário riscado poderia ser um usuário Home (B2E) ou um usuário convidado (B2B, B2C).</span><span class="sxs-lookup"><span data-stu-id="0ed5b-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="0ed5b-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0ed5b-156">isDeleted</span></span>|<span data-ttu-id="0ed5b-157">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0ed5b-157">isDeleted</span></span>| <span data-ttu-id="0ed5b-158">Um usuário pode ou não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="0ed5b-159">riskState</span><span class="sxs-lookup"><span data-stu-id="0ed5b-159">riskState</span></span>|<span data-ttu-id="0ed5b-160">riskState</span><span class="sxs-lookup"><span data-stu-id="0ed5b-160">riskState</span></span>| <span data-ttu-id="0ed5b-161">Um usuário riscado pode existir em um dos vários estados.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="0ed5b-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0ed5b-162">riskDetail</span></span>|<span data-ttu-id="0ed5b-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0ed5b-163">riskDetail</span></span>| <span data-ttu-id="0ed5b-164">Um usuário riscado poderia ser em um determinado estado por vários motivos.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="0ed5b-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0ed5b-165">riskLevel</span></span>|<span data-ttu-id="0ed5b-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0ed5b-166">riskLevel</span></span>| <span data-ttu-id="0ed5b-167">Um usuário riscado poderia ser considerado um dos vários níveis de risco.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ed5b-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ed5b-168">JSON representation</span></span>

<span data-ttu-id="0ed5b-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ed5b-169">Here is a JSON representation of the resource.</span></span>

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
