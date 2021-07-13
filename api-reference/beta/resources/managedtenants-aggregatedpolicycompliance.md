---
title: Tipo de recurso aggregatedPolicyCompliance
description: Representa uma exibição agregada da conformidade do dispositivo para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 8b2c6ce85c0ec6df361ddfeb13a851740efb2acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401947"
---
# <a name="aggregatedpolicycompliance-resource-type"></a><span data-ttu-id="59800-103">Tipo de recurso aggregatedPolicyCompliance</span><span class="sxs-lookup"><span data-stu-id="59800-103">aggregatedPolicyCompliance resource type</span></span>

<span data-ttu-id="59800-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="59800-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59800-105">Representa uma exibição agregada da conformidade do dispositivo para um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="59800-105">Represents an aggregate view of device compliance for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="59800-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="59800-106">Methods</span></span>
|<span data-ttu-id="59800-107">Método</span><span class="sxs-lookup"><span data-stu-id="59800-107">Method</span></span>|<span data-ttu-id="59800-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="59800-108">Return type</span></span>|<span data-ttu-id="59800-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="59800-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59800-110">Listar aggregatedPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="59800-110">List aggregatedPolicyCompliances</span></span>](../api/managedtenants-managedtenant-list-aggregatedpolicycompliances.md)|<span data-ttu-id="59800-111">[coleção microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)</span><span class="sxs-lookup"><span data-stu-id="59800-111">[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) collection</span></span>|<span data-ttu-id="59800-112">Obter uma lista dos [objetos aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="59800-112">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="59800-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59800-113">Properties</span></span>
|<span data-ttu-id="59800-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59800-114">Property</span></span>|<span data-ttu-id="59800-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="59800-115">Type</span></span>|<span data-ttu-id="59800-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="59800-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59800-117">compliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="59800-117">compliancePolicyId</span></span>|<span data-ttu-id="59800-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59800-118">String</span></span>|<span data-ttu-id="59800-119">Identificador da política de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59800-119">Identifier for the device compliance policy.</span></span> <span data-ttu-id="59800-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-120">Optional.</span></span> <span data-ttu-id="59800-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-121">Read-only.</span></span>|
|<span data-ttu-id="59800-122">compliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="59800-122">compliancePolicyName</span></span>|<span data-ttu-id="59800-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59800-123">String</span></span>|<span data-ttu-id="59800-124">Nome da política de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59800-124">Name of the device compliance policy.</span></span> <span data-ttu-id="59800-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-125">Optional.</span></span> <span data-ttu-id="59800-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-126">Read-only.</span></span>|
|<span data-ttu-id="59800-127">compliancePolicyPlatform</span><span class="sxs-lookup"><span data-stu-id="59800-127">compliancePolicyPlatform</span></span>|<span data-ttu-id="59800-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59800-128">String</span></span>|<span data-ttu-id="59800-129">Plataforma para a política de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59800-129">Platform for the device compliance policy.</span></span> <span data-ttu-id="59800-130">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidAOSP`, `all`.</span><span class="sxs-lookup"><span data-stu-id="59800-130">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidAOSP`, `all`.</span></span> <span data-ttu-id="59800-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-131">Optional.</span></span> <span data-ttu-id="59800-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-132">Read-only.</span></span>|
|<span data-ttu-id="59800-133">compliancePolicyType</span><span class="sxs-lookup"><span data-stu-id="59800-133">compliancePolicyType</span></span>|<span data-ttu-id="59800-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59800-134">String</span></span>|<span data-ttu-id="59800-135">O tipo de política de conformidade.</span><span class="sxs-lookup"><span data-stu-id="59800-135">The type of compliance policy.</span></span> <span data-ttu-id="59800-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-136">Optional.</span></span> <span data-ttu-id="59800-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-137">Read-only.</span></span>|
|<span data-ttu-id="59800-138">id</span><span class="sxs-lookup"><span data-stu-id="59800-138">id</span></span>|<span data-ttu-id="59800-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59800-139">String</span></span>|<span data-ttu-id="59800-140">Identificador exclusivo da política de conformidade do dispositivo agregado.</span><span class="sxs-lookup"><span data-stu-id="59800-140">Unique identifier for the aggregate device compliance policy.</span></span> <span data-ttu-id="59800-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59800-141">Required.</span></span> <span data-ttu-id="59800-142">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="59800-142">Read-only</span></span>|
|<span data-ttu-id="59800-143">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="59800-143">lastRefreshedDateTime</span></span>|<span data-ttu-id="59800-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59800-144">DateTimeOffset</span></span>|<span data-ttu-id="59800-145">Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="59800-145">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="59800-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-146">Optional.</span></span> <span data-ttu-id="59800-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-147">Read-only.</span></span>|
|<span data-ttu-id="59800-148">numberOfCompliantDevices</span><span class="sxs-lookup"><span data-stu-id="59800-148">numberOfCompliantDevices</span></span>|<span data-ttu-id="59800-149">Int64</span><span class="sxs-lookup"><span data-stu-id="59800-149">Int64</span></span>|<span data-ttu-id="59800-150">O número de dispositivos que estão em um status compatível.</span><span class="sxs-lookup"><span data-stu-id="59800-150">The number of devices that are in a compliant status.</span></span> <span data-ttu-id="59800-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-151">Optional.</span></span> <span data-ttu-id="59800-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-152">Read-only.</span></span>|
|<span data-ttu-id="59800-153">numberOfErrorDevices</span><span class="sxs-lookup"><span data-stu-id="59800-153">numberOfErrorDevices</span></span>|<span data-ttu-id="59800-154">Int64</span><span class="sxs-lookup"><span data-stu-id="59800-154">Int64</span></span>|<span data-ttu-id="59800-155">O número de dispositivos que estão em um status de erro.</span><span class="sxs-lookup"><span data-stu-id="59800-155">The number of devices that are in an error status.</span></span> <span data-ttu-id="59800-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-156">Optional.</span></span> <span data-ttu-id="59800-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-157">Read-only.</span></span>|
|<span data-ttu-id="59800-158">numberOfNonCompliantDevices</span><span class="sxs-lookup"><span data-stu-id="59800-158">numberOfNonCompliantDevices</span></span>|<span data-ttu-id="59800-159">Int64</span><span class="sxs-lookup"><span data-stu-id="59800-159">Int64</span></span>|<span data-ttu-id="59800-160">O número de dispositivos que estão em um status não compatível.</span><span class="sxs-lookup"><span data-stu-id="59800-160">The number of device that are in a non-compliant status.</span></span> <span data-ttu-id="59800-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-161">Optional.</span></span> <span data-ttu-id="59800-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-162">Read-only.</span></span>|
|<span data-ttu-id="59800-163">policyModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59800-163">policyModifiedDateTime</span></span>|<span data-ttu-id="59800-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59800-164">DateTimeOffset</span></span>|<span data-ttu-id="59800-165">A data e a hora em que a política do dispositivo foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="59800-165">The date and time the device policy was last modified.</span></span> <span data-ttu-id="59800-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-166">Optional.</span></span> <span data-ttu-id="59800-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-167">Read-only.</span></span>|
|<span data-ttu-id="59800-168">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="59800-168">tenantDisplayName</span></span>|<span data-ttu-id="59800-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59800-169">String</span></span>|<span data-ttu-id="59800-170">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="59800-170">The display name for the managed tenant.</span></span> <span data-ttu-id="59800-171">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-171">Optional.</span></span> <span data-ttu-id="59800-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-172">Read-only.</span></span>|
|<span data-ttu-id="59800-173">tenantId</span><span class="sxs-lookup"><span data-stu-id="59800-173">tenantId</span></span>|<span data-ttu-id="59800-174">String</span><span class="sxs-lookup"><span data-stu-id="59800-174">String</span></span>|<span data-ttu-id="59800-175">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="59800-175">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="59800-176">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59800-176">Optional.</span></span> <span data-ttu-id="59800-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59800-177">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59800-178">Relações</span><span class="sxs-lookup"><span data-stu-id="59800-178">Relationships</span></span>
<span data-ttu-id="59800-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59800-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59800-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59800-180">JSON representation</span></span>
<span data-ttu-id="59800-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59800-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "compliancePolicyId": "String",
  "compliancePolicyName": "String",
  "compliancePolicyType": "String",
  "compliancePolicyPlatform": "String",
  "numberOfCompliantDevices": "Integer",
  "numberOfNonCompliantDevices": "Integer",
  "numberOfErrorDevices": "Integer",
  "policyModifiedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
