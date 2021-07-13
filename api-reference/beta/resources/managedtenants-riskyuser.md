---
title: tipo de recurso riskyUser
description: Representa uma conta sinalizada para risco em cada locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3f66998080abcf9580cdd36e0f3e4b24edab2d2d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402142"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="e46fa-103">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="e46fa-103">riskyUser resource type</span></span>

<span data-ttu-id="e46fa-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e46fa-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e46fa-105">Representa uma conta sinalizada para risco em cada locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e46fa-105">Represents an account flagged for risk across each managed tenants.</span></span>

## <a name="methods"></a><span data-ttu-id="e46fa-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e46fa-106">Methods</span></span>
|<span data-ttu-id="e46fa-107">Método</span><span class="sxs-lookup"><span data-stu-id="e46fa-107">Method</span></span>|<span data-ttu-id="e46fa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e46fa-108">Return type</span></span>|<span data-ttu-id="e46fa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e46fa-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e46fa-110">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e46fa-110">List riskyUsers</span></span>](../api/managedtenants-managedtenant-list-riskyusers.md)|<span data-ttu-id="e46fa-111">[coleção microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e46fa-111">[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md) collection</span></span>|<span data-ttu-id="e46fa-112">Obter uma lista dos [objetos riskyUser](../resources/managedtenants-riskyuser.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e46fa-112">Get a list of the [riskyUser](../resources/managedtenants-riskyuser.md) objects and their properties.</span></span>|
|[<span data-ttu-id="e46fa-113">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="e46fa-113">Get riskyUser</span></span>](../api/managedtenants-riskyuser-get.md)|[<span data-ttu-id="e46fa-114">microsoft.graph.managedTenants.riskyUser</span><span class="sxs-lookup"><span data-stu-id="e46fa-114">microsoft.graph.managedTenants.riskyUser</span></span>](../resources/managedtenants-riskyuser.md)|<span data-ttu-id="e46fa-115">Leia as propriedades e as relações de um [objeto riskyUser.](../resources/managedtenants-riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e46fa-115">Read the properties and relationships of a [riskyUser](../resources/managedtenants-riskyuser.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e46fa-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e46fa-116">Properties</span></span>
|<span data-ttu-id="e46fa-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e46fa-117">Property</span></span>|<span data-ttu-id="e46fa-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e46fa-118">Type</span></span>|<span data-ttu-id="e46fa-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e46fa-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e46fa-120">id</span><span class="sxs-lookup"><span data-stu-id="e46fa-120">id</span></span>|<span data-ttu-id="e46fa-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-121">String</span></span>|<span data-ttu-id="e46fa-122">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="e46fa-122">The unique identifier for this entity.</span></span> <span data-ttu-id="e46fa-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e46fa-123">Required.</span></span> <span data-ttu-id="e46fa-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-124">Read-only.</span></span>|
|<span data-ttu-id="e46fa-125">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e46fa-125">isDeleted</span></span>|<span data-ttu-id="e46fa-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e46fa-126">Boolean</span></span>|<span data-ttu-id="e46fa-127">Um sinalizador indicando se a conta foi excluída.</span><span class="sxs-lookup"><span data-stu-id="e46fa-127">A flag indicating whether the account has been deleted.</span></span> <span data-ttu-id="e46fa-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-128">Optional.</span></span> <span data-ttu-id="e46fa-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-129">Read-only.</span></span>|
|<span data-ttu-id="e46fa-130">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="e46fa-130">lastRefreshedDateTime</span></span>|<span data-ttu-id="e46fa-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e46fa-131">DateTimeOffset</span></span>|<span data-ttu-id="e46fa-132">Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="e46fa-132">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="e46fa-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-133">Optional.</span></span> <span data-ttu-id="e46fa-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-134">Read-only.</span></span>|
|<span data-ttu-id="e46fa-135">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e46fa-135">riskDetail</span></span>|<span data-ttu-id="e46fa-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-136">String</span></span>|<span data-ttu-id="e46fa-137">Os detalhes de risco para a conta sinalizada para risco.</span><span class="sxs-lookup"><span data-stu-id="e46fa-137">The risk details for the account flagged for risk.</span></span> <span data-ttu-id="e46fa-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-138">Optional.</span></span> <span data-ttu-id="e46fa-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-139">Read-only.</span></span>|
|<span data-ttu-id="e46fa-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e46fa-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="e46fa-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e46fa-141">DateTimeOffset</span></span>|<span data-ttu-id="e46fa-142">A data e a hora em que as informações de risco foram atualizadas pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e46fa-142">The date and time when the risk information was last updated.</span></span> <span data-ttu-id="e46fa-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-143">Optional.</span></span> <span data-ttu-id="e46fa-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-144">Read-only.</span></span>|
|<span data-ttu-id="e46fa-145">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e46fa-145">riskLevel</span></span>|<span data-ttu-id="e46fa-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-146">String</span></span>|<span data-ttu-id="e46fa-147">O nível de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="e46fa-147">The level of risk that was detected.</span></span> <span data-ttu-id="e46fa-148">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e46fa-148">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="e46fa-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-149">Optional.</span></span> <span data-ttu-id="e46fa-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-150">Read-only.</span></span>|
|<span data-ttu-id="e46fa-151">riskState</span><span class="sxs-lookup"><span data-stu-id="e46fa-151">riskState</span></span>|<span data-ttu-id="e46fa-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-152">String</span></span>|<span data-ttu-id="e46fa-153">O estado de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="e46fa-153">The state of risk that was detected.</span></span> <span data-ttu-id="e46fa-154">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e46fa-154">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="e46fa-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-155">Optional.</span></span> <span data-ttu-id="e46fa-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-156">Read-only.</span></span>|
|<span data-ttu-id="e46fa-157">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="e46fa-157">tenantDisplayName</span></span>|<span data-ttu-id="e46fa-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-158">String</span></span>|<span data-ttu-id="e46fa-159">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e46fa-159">The display name for the managed tenant.</span></span> <span data-ttu-id="e46fa-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-160">Optional.</span></span> <span data-ttu-id="e46fa-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-161">Read-only.</span></span>|
|<span data-ttu-id="e46fa-162">tenantId</span><span class="sxs-lookup"><span data-stu-id="e46fa-162">tenantId</span></span>|<span data-ttu-id="e46fa-163">String</span><span class="sxs-lookup"><span data-stu-id="e46fa-163">String</span></span>|<span data-ttu-id="e46fa-164">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="e46fa-164">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="e46fa-165">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e46fa-165">Required.</span></span> <span data-ttu-id="e46fa-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-166">Read-only.</span></span>|
|<span data-ttu-id="e46fa-167">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e46fa-167">userDisplayName</span></span>|<span data-ttu-id="e46fa-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-168">String</span></span>|<span data-ttu-id="e46fa-169">O nome de exibição da conta onde o risco foi detectado.</span><span class="sxs-lookup"><span data-stu-id="e46fa-169">The display name for the account where risk was detected.</span></span> <span data-ttu-id="e46fa-170">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-170">Optional.</span></span> <span data-ttu-id="e46fa-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-171">Read-only.</span></span>|
|<span data-ttu-id="e46fa-172">userId</span><span class="sxs-lookup"><span data-stu-id="e46fa-172">userId</span></span>|<span data-ttu-id="e46fa-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-173">String</span></span>|<span data-ttu-id="e46fa-174">O identificador da conta de usuário onde o risco foi detectado.</span><span class="sxs-lookup"><span data-stu-id="e46fa-174">The identifier for the user account where risk was detected.</span></span> <span data-ttu-id="e46fa-175">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e46fa-175">Required.</span></span> <span data-ttu-id="e46fa-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-176">Read-only.</span></span>|
|<span data-ttu-id="e46fa-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e46fa-177">userPrincipalName</span></span>|<span data-ttu-id="e46fa-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e46fa-178">String</span></span>|<span data-ttu-id="e46fa-179">O nome principal do usuário (UPN) para a conta onde o risco foi detectado.</span><span class="sxs-lookup"><span data-stu-id="e46fa-179">The user principal name (UPN) for the account where risk was detected.</span></span> <span data-ttu-id="e46fa-180">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e46fa-180">Optional.</span></span> <span data-ttu-id="e46fa-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e46fa-181">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e46fa-182">Relações</span><span class="sxs-lookup"><span data-stu-id="e46fa-182">Relationships</span></span>
<span data-ttu-id="e46fa-183">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e46fa-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e46fa-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e46fa-184">JSON representation</span></span>
<span data-ttu-id="e46fa-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e46fa-185">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
  "id": "String (identifier)",
  "userId": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "isDeleted": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
