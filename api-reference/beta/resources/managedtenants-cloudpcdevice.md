---
title: Tipo de recurso cloudPcDevice
description: Representa um dispositivo de computador na nuvem que pertence a um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 57eabb6720987a8a9bfca4c18e283057848b65cf
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401945"
---
# <a name="cloudpcdevice-resource-type"></a><span data-ttu-id="20b81-103">Tipo de recurso cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="20b81-103">cloudPcDevice resource type</span></span>

<span data-ttu-id="20b81-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="20b81-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20b81-105">Representa um dispositivo de computador na nuvem que pertence a um determinado locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="20b81-105">Represents a cloud PC device that belongs to a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="20b81-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="20b81-106">Methods</span></span>
|<span data-ttu-id="20b81-107">Método</span><span class="sxs-lookup"><span data-stu-id="20b81-107">Method</span></span>|<span data-ttu-id="20b81-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="20b81-108">Return type</span></span>|<span data-ttu-id="20b81-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="20b81-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="20b81-110">Listar cloudPcDevices</span><span class="sxs-lookup"><span data-stu-id="20b81-110">List cloudPcDevices</span></span>](../api/managedtenants-managedtenant-list-cloudpcdevices.md)|<span data-ttu-id="20b81-111">[coleção microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)</span><span class="sxs-lookup"><span data-stu-id="20b81-111">[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) collection</span></span>|<span data-ttu-id="20b81-112">Obter uma lista dos objetos [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="20b81-112">Get a list of the [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects and their properties.</span></span>|
|[<span data-ttu-id="20b81-113">Obter cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="20b81-113">Get cloudPcDevice</span></span>](../api/managedtenants-cloudpcdevice-get.md)|[<span data-ttu-id="20b81-114">microsoft.graph.managedTenants.cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="20b81-114">microsoft.graph.managedTenants.cloudPcDevice</span></span>](../resources/managedtenants-cloudpcdevice.md)|<span data-ttu-id="20b81-115">Leia as propriedades e as relações de um [objeto cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)</span><span class="sxs-lookup"><span data-stu-id="20b81-115">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="20b81-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20b81-116">Properties</span></span>
|<span data-ttu-id="20b81-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20b81-117">Property</span></span>|<span data-ttu-id="20b81-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="20b81-118">Type</span></span>|<span data-ttu-id="20b81-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="20b81-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20b81-120">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="20b81-120">cloudPcStatus</span></span>|<span data-ttu-id="20b81-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-121">String</span></span>|<span data-ttu-id="20b81-122">O status do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-122">The status of the cloud PC.</span></span> <span data-ttu-id="20b81-123">Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="20b81-123">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span> <span data-ttu-id="20b81-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-124">Required.</span></span> <span data-ttu-id="20b81-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-125">Read-only.</span></span>|
|<span data-ttu-id="20b81-126">displayName</span><span class="sxs-lookup"><span data-stu-id="20b81-126">displayName</span></span>|<span data-ttu-id="20b81-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-127">String</span></span>|<span data-ttu-id="20b81-128">O nome de exibição do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-128">The display name for the cloud PC.</span></span> <span data-ttu-id="20b81-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-129">Required.</span></span> <span data-ttu-id="20b81-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-130">Read-only.</span></span>|
|<span data-ttu-id="20b81-131">id</span><span class="sxs-lookup"><span data-stu-id="20b81-131">id</span></span>|<span data-ttu-id="20b81-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-132">String</span></span>|<span data-ttu-id="20b81-133">O identificador exclusivo do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-133">The unique identifier for the cloud PC.</span></span> <span data-ttu-id="20b81-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-134">Required.</span></span> <span data-ttu-id="20b81-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-135">Read-only.</span></span>|
|<span data-ttu-id="20b81-136">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="20b81-136">lastRefreshedDateTime</span></span>|<span data-ttu-id="20b81-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b81-137">DateTimeOffset</span></span>|<span data-ttu-id="20b81-138">Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="20b81-138">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="20b81-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-139">Required.</span></span> <span data-ttu-id="20b81-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-140">Read-only.</span></span>|
|<span data-ttu-id="20b81-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="20b81-141">managedDeviceId</span></span>|<span data-ttu-id="20b81-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-142">String</span></span>|<span data-ttu-id="20b81-143">O identificador de dispositivo gerenciado para o computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-143">The managed device identifier for the cloud PC.</span></span> <span data-ttu-id="20b81-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="20b81-144">Optional.</span></span> <span data-ttu-id="20b81-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-145">Read-only.</span></span>|
|<span data-ttu-id="20b81-146">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="20b81-146">managedDeviceName</span></span>|<span data-ttu-id="20b81-147">String</span><span class="sxs-lookup"><span data-stu-id="20b81-147">String</span></span>|<span data-ttu-id="20b81-148">O nome de exibição do dispositivo gerenciado para o computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-148">The managed device display name for the cloud PC.</span></span> <span data-ttu-id="20b81-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="20b81-149">Optional.</span></span> <span data-ttu-id="20b81-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-150">Read-only.</span></span>|
|<span data-ttu-id="20b81-151">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="20b81-151">provisioningPolicyId</span></span>|<span data-ttu-id="20b81-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-152">String</span></span>|<span data-ttu-id="20b81-153">O identificador de política de provisionamento para o computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-153">The provisioning policy identifier for the cloud PC.</span></span> <span data-ttu-id="20b81-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-154">Required.</span></span> <span data-ttu-id="20b81-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-155">Read-only.</span></span>|
|<span data-ttu-id="20b81-156">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="20b81-156">servicePlanName</span></span>|<span data-ttu-id="20b81-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-157">String</span></span>|<span data-ttu-id="20b81-158">O nome do plano de serviço para o computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-158">The service plan name for the cloud PC.</span></span> <span data-ttu-id="20b81-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-159">Required.</span></span> <span data-ttu-id="20b81-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-160">Read-only.</span></span>|
|<span data-ttu-id="20b81-161">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="20b81-161">tenantDisplayName</span></span>|<span data-ttu-id="20b81-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-162">String</span></span>|<span data-ttu-id="20b81-163">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="20b81-163">The display name for the managed tenant.</span></span> <span data-ttu-id="20b81-164">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-164">Required.</span></span> <span data-ttu-id="20b81-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-165">Read-only.</span></span>|
|<span data-ttu-id="20b81-166">tenantId</span><span class="sxs-lookup"><span data-stu-id="20b81-166">tenantId</span></span>|<span data-ttu-id="20b81-167">String</span><span class="sxs-lookup"><span data-stu-id="20b81-167">String</span></span>|<span data-ttu-id="20b81-168">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="20b81-168">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="20b81-169">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-169">Required.</span></span> <span data-ttu-id="20b81-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-170">Read-only.</span></span>|
|<span data-ttu-id="20b81-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="20b81-171">userPrincipalName</span></span>|<span data-ttu-id="20b81-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b81-172">String</span></span>|<span data-ttu-id="20b81-173">O nome principal do usuário (UPN) do usuário atribuído ao computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="20b81-173">The user principal name (UPN) of the user assigned to the cloud PC.</span></span> <span data-ttu-id="20b81-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b81-174">Required.</span></span> <span data-ttu-id="20b81-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b81-175">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20b81-176">Relações</span><span class="sxs-lookup"><span data-stu-id="20b81-176">Relationships</span></span>
<span data-ttu-id="20b81-177">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20b81-177">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20b81-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20b81-178">JSON representation</span></span>
<span data-ttu-id="20b81-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20b81-179">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "servicePlanName": "String",
  "cloudPcStatus": "String",
  "provisioningPolicyId": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
