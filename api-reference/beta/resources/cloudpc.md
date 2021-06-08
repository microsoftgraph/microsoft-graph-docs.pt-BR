---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 232ad6a8de6634f028ec59080114110c902ce184
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787496"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="6c37b-103">Tipo de recurso cloudPC</span><span class="sxs-lookup"><span data-stu-id="6c37b-103">cloudPC resource type</span></span>

<span data-ttu-id="6c37b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c37b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c37b-105">Representa uma área de trabalho virtual gerenciada pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="6c37b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c37b-106">Methods</span></span>

|<span data-ttu-id="6c37b-107">Método</span><span class="sxs-lookup"><span data-stu-id="6c37b-107">Method</span></span>|<span data-ttu-id="6c37b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c37b-108">Return type</span></span>|<span data-ttu-id="6c37b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c37b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c37b-110">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="6c37b-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="6c37b-111">[Coleção cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="6c37b-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="6c37b-112">Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="6c37b-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="6c37b-113">Obter cloudPC</span><span class="sxs-lookup"><span data-stu-id="6c37b-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="6c37b-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="6c37b-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="6c37b-115">Leia as propriedades e as relações de um [objeto cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="6c37b-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="6c37b-116">Reprovision</span><span class="sxs-lookup"><span data-stu-id="6c37b-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="6c37b-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6c37b-117">None</span></span>|<span data-ttu-id="6c37b-118">Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="6c37b-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c37b-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c37b-119">Properties</span></span>

|<span data-ttu-id="6c37b-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c37b-120">Property</span></span>|<span data-ttu-id="6c37b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c37b-121">Type</span></span>|<span data-ttu-id="6c37b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c37b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c37b-123">id</span><span class="sxs-lookup"><span data-stu-id="6c37b-123">id</span></span>|<span data-ttu-id="6c37b-124">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-124">String</span></span>|<span data-ttu-id="6c37b-125">Identificador exclusivo para o computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="6c37b-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6c37b-126">Read-only.</span></span>|
|<span data-ttu-id="6c37b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="6c37b-127">displayName</span></span>|<span data-ttu-id="6c37b-128">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-128">String</span></span>|<span data-ttu-id="6c37b-129">O nome de exibição do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="6c37b-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="6c37b-130">imageDisplayName</span></span>|<span data-ttu-id="6c37b-131">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-131">String</span></span>|<span data-ttu-id="6c37b-132">Nome da imagem do sistema operacional que está no computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="6c37b-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="6c37b-133">managedDeviceId</span></span>|<span data-ttu-id="6c37b-134">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-134">String</span></span>|<span data-ttu-id="6c37b-135">A ID do dispositivo Intune do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="6c37b-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="6c37b-136">managedDeviceName</span></span>|<span data-ttu-id="6c37b-137">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-137">String</span></span>|<span data-ttu-id="6c37b-138">O nome do dispositivo Intune do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="6c37b-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="6c37b-139">provisioningPolicyId</span></span>|<span data-ttu-id="6c37b-140">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-140">String</span></span>|<span data-ttu-id="6c37b-141">ID da política de provisionamento do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="6c37b-142">provisioningPolicyName</span><span class="sxs-lookup"><span data-stu-id="6c37b-142">provisioningPolicyName</span></span>|<span data-ttu-id="6c37b-143">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-143">String</span></span>|<span data-ttu-id="6c37b-144">A política de provisionamento que é aplicada durante o provisionamento de PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-144">The provisioning policy that is applied during provisioning of cloud PCs.</span></span>|
|<span data-ttu-id="6c37b-145">onPremisesConnectionName</span><span class="sxs-lookup"><span data-stu-id="6c37b-145">onPremisesConnectionName</span></span>|<span data-ttu-id="6c37b-146">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-146">String</span></span>|<span data-ttu-id="6c37b-147">A conexão local que é aplicada durante o provisionamento de PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-147">The on-premises connection that is applied during provisioning of cloud PCs.</span></span>|
|<span data-ttu-id="6c37b-148">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="6c37b-148">servicePlanId</span></span>|<span data-ttu-id="6c37b-149">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-149">String</span></span>|<span data-ttu-id="6c37b-150">ID do plano de serviço do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-150">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="6c37b-151">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="6c37b-151">servicePlanName</span></span>|<span data-ttu-id="6c37b-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c37b-152">String</span></span>|<span data-ttu-id="6c37b-153">O nome do plano de serviço do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-153">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="6c37b-154">status</span><span class="sxs-lookup"><span data-stu-id="6c37b-154">status</span></span>|[<span data-ttu-id="6c37b-155">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="6c37b-155">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="6c37b-156">Status do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-156">Status of the cloud PC.</span></span> <span data-ttu-id="6c37b-157">Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6c37b-157">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="6c37b-158">statusDetails</span><span class="sxs-lookup"><span data-stu-id="6c37b-158">statusDetails</span></span>|[<span data-ttu-id="6c37b-159">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="6c37b-159">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="6c37b-160">Os detalhes do status do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-160">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="6c37b-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c37b-161">userPrincipalName</span></span>|<span data-ttu-id="6c37b-162">String</span><span class="sxs-lookup"><span data-stu-id="6c37b-162">String</span></span>|<span data-ttu-id="6c37b-163">O nome principal do usuário (UPN) do usuário atribuído ao computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-163">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="6c37b-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c37b-164">lastModifiedDateTime</span></span>|<span data-ttu-id="6c37b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c37b-165">DateTimeOffset</span></span>|<span data-ttu-id="6c37b-166">Data e hora da última modificação do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="6c37b-166">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="6c37b-167">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6c37b-167">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c37b-168">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6c37b-168">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="6c37b-169">gracePeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="6c37b-169">gracePeriodEndDateTime</span></span>|<span data-ttu-id="6c37b-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c37b-170">DateTimeOffset</span></span>|<span data-ttu-id="6c37b-171">A data e a hora em que o período de carência termina e o reprovisionamento/desprovisionamento acontece.</span><span class="sxs-lookup"><span data-stu-id="6c37b-171">The date and time when the grace period ends and reprovisioning/deprovisioning happens.</span></span> <span data-ttu-id="6c37b-172">Obrigatório somente se o status for `inGracePeriod` .</span><span class="sxs-lookup"><span data-stu-id="6c37b-172">Required only if status is `inGracePeriod`.</span></span> <span data-ttu-id="6c37b-173">O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="6c37b-173">The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="6c37b-174">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6c37b-174">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="6c37b-175">valores cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="6c37b-175">cloudPcStatus values</span></span>

|<span data-ttu-id="6c37b-176">Member</span><span class="sxs-lookup"><span data-stu-id="6c37b-176">Member</span></span>|<span data-ttu-id="6c37b-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c37b-177">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c37b-178">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="6c37b-178">notProvisioned</span></span>|<span data-ttu-id="6c37b-179">O Cloud PC não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="6c37b-179">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="6c37b-180">provisionamento</span><span class="sxs-lookup"><span data-stu-id="6c37b-180">provisioning</span></span>|<span data-ttu-id="6c37b-181">Cloud PC provisionamento está em andamento.</span><span class="sxs-lookup"><span data-stu-id="6c37b-181">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="6c37b-182">provisionado</span><span class="sxs-lookup"><span data-stu-id="6c37b-182">provisioned</span></span>|<span data-ttu-id="6c37b-183">O Cloud PC é provisionado e pode ser acessado por usuários finais.</span><span class="sxs-lookup"><span data-stu-id="6c37b-183">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="6c37b-184">atualização</span><span class="sxs-lookup"><span data-stu-id="6c37b-184">upgrading</span></span>|<span data-ttu-id="6c37b-185">Cloud PC resize está em andamento.</span><span class="sxs-lookup"><span data-stu-id="6c37b-185">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="6c37b-186">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="6c37b-186">inGracePeriod</span></span>|<span data-ttu-id="6c37b-187">O Cloud PC está no período de carência de uma semana antes de ser desprovisionado.</span><span class="sxs-lookup"><span data-stu-id="6c37b-187">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="6c37b-188">desprovisionamento</span><span class="sxs-lookup"><span data-stu-id="6c37b-188">deprovisioning</span></span>|<span data-ttu-id="6c37b-189">O Cloud PC está desprovisionando.</span><span class="sxs-lookup"><span data-stu-id="6c37b-189">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="6c37b-190">failed</span><span class="sxs-lookup"><span data-stu-id="6c37b-190">failed</span></span>|<span data-ttu-id="6c37b-191">A operação em Cloud PC falhou.</span><span class="sxs-lookup"><span data-stu-id="6c37b-191">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c37b-192">Relações</span><span class="sxs-lookup"><span data-stu-id="6c37b-192">Relationships</span></span>

<span data-ttu-id="6c37b-193">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c37b-193">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c37b-194">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c37b-194">JSON representation</span></span>

<span data-ttu-id="6c37b-195">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c37b-195">The following is a JSON representation of the resource.</span></span>
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
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)"
}
```
