---
title: Tipo de recurso riskyUserHistoryItem
description: item de histórico de usuário arriscado
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2188a3a13d36a6d224b3c8ca2a7ac297c22712ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443885"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="32ee0-103">Tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="32ee0-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="32ee0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32ee0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32ee0-105">Representa o histórico de risco de um usuário do Azure AD, conforme determinado pela Proteção de Identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="32ee0-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="32ee0-106">Herda de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="32ee0-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="32ee0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="32ee0-107">Methods</span></span>
|<span data-ttu-id="32ee0-108">Método</span><span class="sxs-lookup"><span data-stu-id="32ee0-108">Method</span></span>|<span data-ttu-id="32ee0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="32ee0-109">Return type</span></span>|<span data-ttu-id="32ee0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="32ee0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32ee0-111">Histórico de listas</span><span class="sxs-lookup"><span data-stu-id="32ee0-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="32ee0-112">[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="32ee0-113">Obter os riskyUserHistoryItems da propriedade de navegação histórico.</span><span class="sxs-lookup"><span data-stu-id="32ee0-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="32ee0-114">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="32ee0-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="32ee0-115">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="32ee0-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="32ee0-116">Leia as propriedades e as relações de um [objeto riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="32ee0-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32ee0-117">Properties</span></span>
|<span data-ttu-id="32ee0-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32ee0-118">Property</span></span>|<span data-ttu-id="32ee0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="32ee0-119">Type</span></span>|<span data-ttu-id="32ee0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="32ee0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32ee0-121">atividade</span><span class="sxs-lookup"><span data-stu-id="32ee0-121">activity</span></span>|[<span data-ttu-id="32ee0-122">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="32ee0-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="32ee0-123">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="32ee0-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="32ee0-124">id</span><span class="sxs-lookup"><span data-stu-id="32ee0-124">id</span></span>|<span data-ttu-id="32ee0-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32ee0-125">String</span></span>|<span data-ttu-id="32ee0-126">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="32ee0-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="32ee0-127">initiatedBy</span></span>|<span data-ttu-id="32ee0-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32ee0-128">String</span></span>|<span data-ttu-id="32ee0-129">A id do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="32ee0-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="32ee0-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="32ee0-130">isDeleted</span></span>|<span data-ttu-id="32ee0-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="32ee0-131">Boolean</span></span>| <span data-ttu-id="32ee0-132">Herdado [de riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="32ee0-133">isProcessing</span><span class="sxs-lookup"><span data-stu-id="32ee0-133">isProcessing</span></span>|<span data-ttu-id="32ee0-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="32ee0-134">Boolean</span></span>| <span data-ttu-id="32ee0-135">Herdado [de riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="32ee0-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="32ee0-136">riskDetail</span></span>|<span data-ttu-id="32ee0-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="32ee0-137">riskDetail</span></span>|<span data-ttu-id="32ee0-138">Herdado [de riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="32ee0-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="32ee0-139">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="32ee0-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="32ee0-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="32ee0-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="32ee0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32ee0-141">DateTimeOffset</span></span>|<span data-ttu-id="32ee0-142">Herdado [de riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="32ee0-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="32ee0-143">riskLevel</span></span>|<span data-ttu-id="32ee0-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="32ee0-144">riskLevel</span></span>|<span data-ttu-id="32ee0-145">Herdado [de riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="32ee0-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="32ee0-146">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="32ee0-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="32ee0-147">riskState</span><span class="sxs-lookup"><span data-stu-id="32ee0-147">riskState</span></span>|<span data-ttu-id="32ee0-148">riskState</span><span class="sxs-lookup"><span data-stu-id="32ee0-148">riskState</span></span>|<span data-ttu-id="32ee0-149">Herdado [de riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="32ee0-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="32ee0-150">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="32ee0-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="32ee0-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="32ee0-151">userDisplayName</span></span>|<span data-ttu-id="32ee0-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32ee0-152">String</span></span>|<span data-ttu-id="32ee0-153">Herdado [de riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="32ee0-154">userId</span><span class="sxs-lookup"><span data-stu-id="32ee0-154">userId</span></span>|<span data-ttu-id="32ee0-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32ee0-155">String</span></span>|<span data-ttu-id="32ee0-156">A id do usuário.</span><span class="sxs-lookup"><span data-stu-id="32ee0-156">The id of the user.</span></span>|
|<span data-ttu-id="32ee0-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="32ee0-157">userPrincipalName</span></span>|<span data-ttu-id="32ee0-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32ee0-158">String</span></span>|<span data-ttu-id="32ee0-159">Nome principal do usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="32ee0-159">Risky user principal name.</span></span> <span data-ttu-id="32ee0-160">Herdado [de riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="32ee0-161">Relações</span><span class="sxs-lookup"><span data-stu-id="32ee0-161">Relationships</span></span>
|<span data-ttu-id="32ee0-162">Relação</span><span class="sxs-lookup"><span data-stu-id="32ee0-162">Relationship</span></span>|<span data-ttu-id="32ee0-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="32ee0-163">Type</span></span>|<span data-ttu-id="32ee0-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="32ee0-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32ee0-165">history</span><span class="sxs-lookup"><span data-stu-id="32ee0-165">history</span></span>|<span data-ttu-id="32ee0-166">[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="32ee0-167">Herdado [de riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="32ee0-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32ee0-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32ee0-168">JSON representation</span></span>
<span data-ttu-id="32ee0-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32ee0-169">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```


