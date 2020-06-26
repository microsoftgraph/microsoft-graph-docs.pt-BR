---
title: tipo de recurso riskyUser
description: item de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0584a0c1c36428cac735f33eb690821e5d045ae3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896004"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="21896-103">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="21896-103">riskyUser resource type</span></span>

<span data-ttu-id="21896-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21896-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21896-105">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="21896-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="21896-106">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="21896-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="21896-107">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="21896-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="21896-108">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="21896-108">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="21896-109">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="21896-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="21896-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="21896-110">Methods</span></span>
|<span data-ttu-id="21896-111">Método</span><span class="sxs-lookup"><span data-stu-id="21896-111">Method</span></span>|<span data-ttu-id="21896-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="21896-112">Return type</span></span>|<span data-ttu-id="21896-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="21896-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21896-114">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="21896-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="21896-115">coleção [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="21896-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="21896-116">Obtenha uma lista dos objetos **riskyUser** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="21896-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="21896-117">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="21896-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="21896-118">riskyUser</span><span class="sxs-lookup"><span data-stu-id="21896-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="21896-119">Leia as propriedades e os relacionamentos de um objeto **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="21896-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="21896-120">Ignorar um riskyUser</span><span class="sxs-lookup"><span data-stu-id="21896-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="21896-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21896-121">None</span></span>|<span data-ttu-id="21896-122">Descarte o risco de um ou mais objetos **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="21896-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="21896-123">Confirmar um riskyUser como comprometido</span><span class="sxs-lookup"><span data-stu-id="21896-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="21896-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21896-124">None</span></span>|<span data-ttu-id="21896-125">Confirme um ou mais objetos **riskyUser** como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="21896-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="21896-126">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="21896-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="21896-127">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="21896-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="21896-128">Obtenha o **riskyUserHistoryItems** da propriedade de navegação History.</span><span class="sxs-lookup"><span data-stu-id="21896-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="21896-129">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="21896-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="21896-130">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="21896-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="21896-131">Leia as propriedades e os relacionamentos de um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="21896-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="21896-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21896-132">Properties</span></span>
|<span data-ttu-id="21896-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21896-133">Property</span></span>|<span data-ttu-id="21896-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="21896-134">Type</span></span>|<span data-ttu-id="21896-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="21896-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21896-136">id</span><span class="sxs-lookup"><span data-stu-id="21896-136">id</span></span>|<span data-ttu-id="21896-137">String</span><span class="sxs-lookup"><span data-stu-id="21896-137">String</span></span>|<span data-ttu-id="21896-138">ID exclusiva do usuário em risco.</span><span class="sxs-lookup"><span data-stu-id="21896-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="21896-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="21896-139">isDeleted</span></span>|<span data-ttu-id="21896-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="21896-140">Boolean</span></span>|<span data-ttu-id="21896-141">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="21896-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="21896-142">Os valores possíveis são: `true` ,`false`</span><span class="sxs-lookup"><span data-stu-id="21896-142">Possible values are: `true`, `false`</span></span>|
|<span data-ttu-id="21896-143">isprocessoing</span><span class="sxs-lookup"><span data-stu-id="21896-143">isProcessing</span></span>|<span data-ttu-id="21896-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="21896-144">Boolean</span></span>|<span data-ttu-id="21896-145">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="21896-145">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|<span data-ttu-id="21896-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="21896-146">riskDetail</span></span>|<span data-ttu-id="21896-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="21896-147">riskDetail</span></span>|<span data-ttu-id="21896-148">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="21896-148">Details of the detected risk.</span></span> <span data-ttu-id="21896-149">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21896-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21896-150">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="21896-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="21896-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21896-151">DateTimeOffset</span></span>|<span data-ttu-id="21896-152">A data e a hora em que o usuário arriscado foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="21896-152">The date and time that the risky user was last updated.</span></span>|
|<span data-ttu-id="21896-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="21896-153">riskLevel</span></span>|<span data-ttu-id="21896-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="21896-154">riskLevel</span></span>|<span data-ttu-id="21896-155">Nível do usuário arriscado detectado.</span><span class="sxs-lookup"><span data-stu-id="21896-155">Level of the detected risky user.</span></span> <span data-ttu-id="21896-156">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21896-156">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21896-157">riskState</span><span class="sxs-lookup"><span data-stu-id="21896-157">riskState</span></span>|<span data-ttu-id="21896-158">riskState</span><span class="sxs-lookup"><span data-stu-id="21896-158">riskState</span></span>|<span data-ttu-id="21896-159">Estado do risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="21896-159">State of the user's risk.</span></span> <span data-ttu-id="21896-160">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21896-160">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21896-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="21896-161">userDisplayName</span></span>|<span data-ttu-id="21896-162">String</span><span class="sxs-lookup"><span data-stu-id="21896-162">String</span></span>|<span data-ttu-id="21896-163">Nome de exibição do usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="21896-163">Risky user display name.</span></span>|
|<span data-ttu-id="21896-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21896-164">userPrincipalName</span></span>|<span data-ttu-id="21896-165">String</span><span class="sxs-lookup"><span data-stu-id="21896-165">String</span></span>|<span data-ttu-id="21896-166">Nome UPN de usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="21896-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21896-167">Relações</span><span class="sxs-lookup"><span data-stu-id="21896-167">Relationships</span></span>
|<span data-ttu-id="21896-168">Relação</span><span class="sxs-lookup"><span data-stu-id="21896-168">Relationship</span></span>|<span data-ttu-id="21896-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="21896-169">Type</span></span>|<span data-ttu-id="21896-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="21896-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21896-171">histórico</span><span class="sxs-lookup"><span data-stu-id="21896-171">history</span></span>|<span data-ttu-id="21896-172">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="21896-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="21896-173">A atividade relacionada à alteração no nível de risco do usuário</span><span class="sxs-lookup"><span data-stu-id="21896-173">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21896-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21896-174">JSON representation</span></span>
<span data-ttu-id="21896-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21896-175">The following is a JSON representation of the resource.</span></span>
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

