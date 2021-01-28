---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b026bccd18af0dcbc9c0a5128595399a0997474
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033915"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="c25ab-103">Tipo de recurso cloudPC</span><span class="sxs-lookup"><span data-stu-id="c25ab-103">cloudPC resource type</span></span>

<span data-ttu-id="c25ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c25ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c25ab-105">Representa uma área de trabalho virtual gerenciada na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="c25ab-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c25ab-106">Methods</span></span>

|<span data-ttu-id="c25ab-107">Método</span><span class="sxs-lookup"><span data-stu-id="c25ab-107">Method</span></span>|<span data-ttu-id="c25ab-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c25ab-108">Return type</span></span>|<span data-ttu-id="c25ab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c25ab-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c25ab-110">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="c25ab-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="c25ab-111">[Coleção cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="c25ab-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="c25ab-112">Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="c25ab-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="c25ab-113">Obter cloudPC</span><span class="sxs-lookup"><span data-stu-id="c25ab-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="c25ab-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="c25ab-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="c25ab-115">Leia as propriedades e os relacionamentos de um [objeto cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="c25ab-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="c25ab-116">Reprovisionamento</span><span class="sxs-lookup"><span data-stu-id="c25ab-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="c25ab-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c25ab-117">None</span></span>|<span data-ttu-id="c25ab-118">Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="c25ab-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c25ab-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c25ab-119">Properties</span></span>

|<span data-ttu-id="c25ab-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c25ab-120">Property</span></span>|<span data-ttu-id="c25ab-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c25ab-121">Type</span></span>|<span data-ttu-id="c25ab-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c25ab-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c25ab-123">id</span><span class="sxs-lookup"><span data-stu-id="c25ab-123">id</span></span>|<span data-ttu-id="c25ab-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-124">String</span></span>|<span data-ttu-id="c25ab-125">Identificador exclusivo do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="c25ab-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c25ab-126">Read-only.</span></span>|
|<span data-ttu-id="c25ab-127">displayName</span><span class="sxs-lookup"><span data-stu-id="c25ab-127">displayName</span></span>|<span data-ttu-id="c25ab-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-128">String</span></span>|<span data-ttu-id="c25ab-129">O nome de exibição do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="c25ab-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="c25ab-130">imageDisplayName</span></span>|<span data-ttu-id="c25ab-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-131">String</span></span>|<span data-ttu-id="c25ab-132">Nome da imagem do sistema operacional que está no computador em nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="c25ab-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c25ab-133">managedDeviceId</span></span>|<span data-ttu-id="c25ab-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-134">String</span></span>|<span data-ttu-id="c25ab-135">A ID do dispositivo Intune do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="c25ab-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c25ab-136">managedDeviceName</span></span>|<span data-ttu-id="c25ab-137">String</span><span class="sxs-lookup"><span data-stu-id="c25ab-137">String</span></span>|<span data-ttu-id="c25ab-138">O nome do dispositivo Intune do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="c25ab-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="c25ab-139">provisioningPolicyId</span></span>|<span data-ttu-id="c25ab-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-140">String</span></span>|<span data-ttu-id="c25ab-141">A ID de política de provisionamento do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="c25ab-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="c25ab-142">servicePlanId</span></span>|<span data-ttu-id="c25ab-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-143">String</span></span>|<span data-ttu-id="c25ab-144">A ID do plano de serviço do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="c25ab-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="c25ab-145">servicePlanName</span></span>|<span data-ttu-id="c25ab-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-146">String</span></span>|<span data-ttu-id="c25ab-147">O nome do plano de serviço do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="c25ab-148">status</span><span class="sxs-lookup"><span data-stu-id="c25ab-148">status</span></span>|[<span data-ttu-id="c25ab-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="c25ab-149">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="c25ab-150">Status do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-150">Status of the cloud PC.</span></span> <span data-ttu-id="c25ab-151">Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c25ab-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="c25ab-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="c25ab-152">statusDetails</span></span>|[<span data-ttu-id="c25ab-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="c25ab-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="c25ab-154">Os detalhes do status do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="c25ab-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c25ab-155">userPrincipalName</span></span>|<span data-ttu-id="c25ab-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c25ab-156">String</span></span>|<span data-ttu-id="c25ab-157">O nome UPN do usuário atribuído ao computador em nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="c25ab-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c25ab-158">lastModifiedDateTime</span></span>|<span data-ttu-id="c25ab-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c25ab-159">DateTimeOffset</span></span>|<span data-ttu-id="c25ab-160">Data e hora da última modificação do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c25ab-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="c25ab-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c25ab-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c25ab-162">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="c25ab-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="c25ab-163">Valores de cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="c25ab-163">cloudPcStatus values</span></span>

|<span data-ttu-id="c25ab-164">Member</span><span class="sxs-lookup"><span data-stu-id="c25ab-164">Member</span></span>|<span data-ttu-id="c25ab-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="c25ab-165">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c25ab-166">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="c25ab-166">notProvisioned</span></span>|<span data-ttu-id="c25ab-167">O Cloud PC não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="c25ab-167">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="c25ab-168">provisionamento</span><span class="sxs-lookup"><span data-stu-id="c25ab-168">provisioning</span></span>|<span data-ttu-id="c25ab-169">O provisionamento de computadores na nuvem está em andamento.</span><span class="sxs-lookup"><span data-stu-id="c25ab-169">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="c25ab-170">provisionado</span><span class="sxs-lookup"><span data-stu-id="c25ab-170">provisioned</span></span>|<span data-ttu-id="c25ab-171">O Cloud PC é provisionado e pode ser acessado por usuários finais.</span><span class="sxs-lookup"><span data-stu-id="c25ab-171">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="c25ab-172">atualização</span><span class="sxs-lookup"><span data-stu-id="c25ab-172">upgrading</span></span>|<span data-ttu-id="c25ab-173">O relize do computador na nuvem está em andamento.</span><span class="sxs-lookup"><span data-stu-id="c25ab-173">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="c25ab-174">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="c25ab-174">inGracePeriod</span></span>|<span data-ttu-id="c25ab-175">O Cloud PC está no período de carência de uma semana antes de ser desprovisionado.</span><span class="sxs-lookup"><span data-stu-id="c25ab-175">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="c25ab-176">desprovisioning</span><span class="sxs-lookup"><span data-stu-id="c25ab-176">deprovisioning</span></span>|<span data-ttu-id="c25ab-177">O Cloud PC está desprovisionamento.</span><span class="sxs-lookup"><span data-stu-id="c25ab-177">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="c25ab-178">failed</span><span class="sxs-lookup"><span data-stu-id="c25ab-178">failed</span></span>|<span data-ttu-id="c25ab-179">A operação no Cloud PC falhou.</span><span class="sxs-lookup"><span data-stu-id="c25ab-179">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c25ab-180">Relações</span><span class="sxs-lookup"><span data-stu-id="c25ab-180">Relationships</span></span>

<span data-ttu-id="c25ab-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c25ab-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c25ab-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c25ab-182">JSON representation</span></span>

<span data-ttu-id="c25ab-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c25ab-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```
