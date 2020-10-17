---
title: tipo de recurso riskyUser
description: item de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2989b0f74243679daaebcb482c0640a78bc9effa
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581285"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="28790-103">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="28790-103">riskyUser resource type</span></span>

<span data-ttu-id="28790-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28790-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28790-105">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="28790-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="28790-106">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="28790-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="28790-107">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28790-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="28790-108">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="28790-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="28790-109">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="28790-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="28790-110">Methods</span><span class="sxs-lookup"><span data-stu-id="28790-110">Methods</span></span>
|<span data-ttu-id="28790-111">Método</span><span class="sxs-lookup"><span data-stu-id="28790-111">Method</span></span>|<span data-ttu-id="28790-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="28790-112">Return type</span></span>|<span data-ttu-id="28790-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="28790-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28790-114">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="28790-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="28790-115">coleção [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="28790-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="28790-116">Obtenha uma lista dos objetos **riskyUser** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="28790-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="28790-117">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="28790-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="28790-118">riskyUser</span><span class="sxs-lookup"><span data-stu-id="28790-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="28790-119">Leia as propriedades e os relacionamentos de um objeto **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="28790-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="28790-120">Ignorar um riskyUser</span><span class="sxs-lookup"><span data-stu-id="28790-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="28790-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28790-121">None</span></span>|<span data-ttu-id="28790-122">Descarte o risco de um ou mais objetos **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="28790-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="28790-123">Confirmar um riskyUser como comprometido</span><span class="sxs-lookup"><span data-stu-id="28790-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="28790-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28790-124">None</span></span>|<span data-ttu-id="28790-125">Confirme um ou mais objetos **riskyUser** como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="28790-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="28790-126">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="28790-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="28790-127">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="28790-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="28790-128">Obtenha o **riskyUserHistoryItems** da propriedade de navegação History.</span><span class="sxs-lookup"><span data-stu-id="28790-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="28790-129">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="28790-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="28790-130">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="28790-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="28790-131">Leia as propriedades e os relacionamentos de um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="28790-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="28790-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28790-132">Properties</span></span>
|<span data-ttu-id="28790-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28790-133">Property</span></span>|<span data-ttu-id="28790-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="28790-134">Type</span></span>|<span data-ttu-id="28790-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="28790-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28790-136">id</span><span class="sxs-lookup"><span data-stu-id="28790-136">id</span></span>|<span data-ttu-id="28790-137">String</span><span class="sxs-lookup"><span data-stu-id="28790-137">String</span></span>|<span data-ttu-id="28790-138">ID exclusiva do usuário em risco.</span><span class="sxs-lookup"><span data-stu-id="28790-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="28790-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="28790-139">isDeleted</span></span>|<span data-ttu-id="28790-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="28790-140">Boolean</span></span>|<span data-ttu-id="28790-141">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="28790-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="28790-142">Os valores possíveis são: `true` , `false`</span><span class="sxs-lookup"><span data-stu-id="28790-142">Possible values are: `true`, `false`</span></span>|
|<span data-ttu-id="28790-143">isprocessoing</span><span class="sxs-lookup"><span data-stu-id="28790-143">isProcessing</span></span>|<span data-ttu-id="28790-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="28790-144">Boolean</span></span>|<span data-ttu-id="28790-145">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="28790-145">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|<span data-ttu-id="28790-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="28790-146">riskDetail</span></span>|<span data-ttu-id="28790-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="28790-147">riskDetail</span></span>|<span data-ttu-id="28790-148">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="28790-148">Details of the detected risk.</span></span> <span data-ttu-id="28790-149">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28790-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="28790-150">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="28790-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="28790-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28790-151">DateTimeOffset</span></span>|<span data-ttu-id="28790-152">A data e a hora em que o usuário arriscado foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="28790-152">The date and time that the risky user was last updated.</span></span>|
|<span data-ttu-id="28790-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="28790-153">riskLevel</span></span>|<span data-ttu-id="28790-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="28790-154">riskLevel</span></span>|<span data-ttu-id="28790-155">Nível do usuário arriscado detectado.</span><span class="sxs-lookup"><span data-stu-id="28790-155">Level of the detected risky user.</span></span> <span data-ttu-id="28790-156">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28790-156">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="28790-157">riskState</span><span class="sxs-lookup"><span data-stu-id="28790-157">riskState</span></span>|<span data-ttu-id="28790-158">riskState</span><span class="sxs-lookup"><span data-stu-id="28790-158">riskState</span></span>|<span data-ttu-id="28790-159">Estado do risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="28790-159">State of the user's risk.</span></span> <span data-ttu-id="28790-160">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28790-160">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="28790-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="28790-161">userDisplayName</span></span>|<span data-ttu-id="28790-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28790-162">String</span></span>|<span data-ttu-id="28790-163">Nome de exibição do usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="28790-163">Risky user display name.</span></span>|
|<span data-ttu-id="28790-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="28790-164">userPrincipalName</span></span>|<span data-ttu-id="28790-165">String</span><span class="sxs-lookup"><span data-stu-id="28790-165">String</span></span>|<span data-ttu-id="28790-166">Nome UPN de usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="28790-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28790-167">Relações</span><span class="sxs-lookup"><span data-stu-id="28790-167">Relationships</span></span>
|<span data-ttu-id="28790-168">Relação</span><span class="sxs-lookup"><span data-stu-id="28790-168">Relationship</span></span>|<span data-ttu-id="28790-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="28790-169">Type</span></span>|<span data-ttu-id="28790-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="28790-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28790-171">histórico</span><span class="sxs-lookup"><span data-stu-id="28790-171">history</span></span>|<span data-ttu-id="28790-172">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="28790-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="28790-173">A atividade relacionada à alteração no nível de risco do usuário</span><span class="sxs-lookup"><span data-stu-id="28790-173">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28790-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28790-174">JSON representation</span></span>
<span data-ttu-id="28790-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28790-175">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```