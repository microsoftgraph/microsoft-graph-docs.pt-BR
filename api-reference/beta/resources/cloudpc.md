---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c5fc858e29abf7d649b32991d9e30ce64cc0b632
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721611"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="34a41-103">Tipo de recurso cloudPC</span><span class="sxs-lookup"><span data-stu-id="34a41-103">cloudPC resource type</span></span>

<span data-ttu-id="34a41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34a41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34a41-105">Representa uma área de trabalho virtual gerenciada pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="34a41-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="34a41-106">Methods</span></span>

|<span data-ttu-id="34a41-107">Método</span><span class="sxs-lookup"><span data-stu-id="34a41-107">Method</span></span>|<span data-ttu-id="34a41-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="34a41-108">Return type</span></span>|<span data-ttu-id="34a41-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34a41-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34a41-110">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="34a41-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="34a41-111">[Coleção cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="34a41-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="34a41-112">Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="34a41-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="34a41-113">Obter cloudPC</span><span class="sxs-lookup"><span data-stu-id="34a41-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="34a41-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="34a41-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="34a41-115">Leia as propriedades e as relações de um [objeto cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="34a41-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="34a41-116">Reprovision</span><span class="sxs-lookup"><span data-stu-id="34a41-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="34a41-117">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="34a41-117">None</span></span>|<span data-ttu-id="34a41-118">Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="34a41-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34a41-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34a41-119">Properties</span></span>

|<span data-ttu-id="34a41-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34a41-120">Property</span></span>|<span data-ttu-id="34a41-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="34a41-121">Type</span></span>|<span data-ttu-id="34a41-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="34a41-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a41-123">id</span><span class="sxs-lookup"><span data-stu-id="34a41-123">id</span></span>|<span data-ttu-id="34a41-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-124">String</span></span>|<span data-ttu-id="34a41-125">Identificador exclusivo para o computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="34a41-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34a41-126">Read-only.</span></span>|
|<span data-ttu-id="34a41-127">displayName</span><span class="sxs-lookup"><span data-stu-id="34a41-127">displayName</span></span>|<span data-ttu-id="34a41-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-128">String</span></span>|<span data-ttu-id="34a41-129">O nome de exibição do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="34a41-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="34a41-130">imageDisplayName</span></span>|<span data-ttu-id="34a41-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-131">String</span></span>|<span data-ttu-id="34a41-132">Nome da imagem do sistema operacional que está no computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="34a41-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="34a41-133">managedDeviceId</span></span>|<span data-ttu-id="34a41-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-134">String</span></span>|<span data-ttu-id="34a41-135">A ID do dispositivo Intune do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="34a41-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="34a41-136">managedDeviceName</span></span>|<span data-ttu-id="34a41-137">String</span><span class="sxs-lookup"><span data-stu-id="34a41-137">String</span></span>|<span data-ttu-id="34a41-138">O nome do dispositivo Intune do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="34a41-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="34a41-139">provisioningPolicyId</span></span>|<span data-ttu-id="34a41-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-140">String</span></span>|<span data-ttu-id="34a41-141">ID da política de provisionamento do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="34a41-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="34a41-142">servicePlanId</span></span>|<span data-ttu-id="34a41-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-143">String</span></span>|<span data-ttu-id="34a41-144">ID do plano de serviço do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="34a41-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="34a41-145">servicePlanName</span></span>|<span data-ttu-id="34a41-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-146">String</span></span>|<span data-ttu-id="34a41-147">O nome do plano de serviço do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="34a41-148">status</span><span class="sxs-lookup"><span data-stu-id="34a41-148">status</span></span>|[<span data-ttu-id="34a41-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="34a41-149">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="34a41-150">Status do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-150">Status of the cloud PC.</span></span> <span data-ttu-id="34a41-151">Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="34a41-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="34a41-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="34a41-152">statusDetails</span></span>|[<span data-ttu-id="34a41-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="34a41-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="34a41-154">Os detalhes do status do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="34a41-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34a41-155">userPrincipalName</span></span>|<span data-ttu-id="34a41-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34a41-156">String</span></span>|<span data-ttu-id="34a41-157">O nome principal do usuário (UPN) do usuário atribuído ao computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="34a41-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34a41-158">lastModifiedDateTime</span></span>|<span data-ttu-id="34a41-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a41-159">DateTimeOffset</span></span>|<span data-ttu-id="34a41-160">Data e hora da última modificação do computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="34a41-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="34a41-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="34a41-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34a41-162">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="34a41-162">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="34a41-163">valores cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="34a41-163">cloudPcStatus values</span></span>

|<span data-ttu-id="34a41-164">Member</span><span class="sxs-lookup"><span data-stu-id="34a41-164">Member</span></span>|<span data-ttu-id="34a41-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="34a41-165">Description</span></span>|
|:---|:---|
|<span data-ttu-id="34a41-166">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="34a41-166">notProvisioned</span></span>|<span data-ttu-id="34a41-167">O Cloud PC não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="34a41-167">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="34a41-168">provisionamento</span><span class="sxs-lookup"><span data-stu-id="34a41-168">provisioning</span></span>|<span data-ttu-id="34a41-169">O provisionamento do computador na nuvem está em andamento.</span><span class="sxs-lookup"><span data-stu-id="34a41-169">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="34a41-170">provisionado</span><span class="sxs-lookup"><span data-stu-id="34a41-170">provisioned</span></span>|<span data-ttu-id="34a41-171">O Cloud PC é provisionado e pode ser acessado por usuários finais.</span><span class="sxs-lookup"><span data-stu-id="34a41-171">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="34a41-172">atualização</span><span class="sxs-lookup"><span data-stu-id="34a41-172">upgrading</span></span>|<span data-ttu-id="34a41-173">O resize do Cloud PC está em andamento.</span><span class="sxs-lookup"><span data-stu-id="34a41-173">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="34a41-174">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="34a41-174">inGracePeriod</span></span>|<span data-ttu-id="34a41-175">O Cloud PC está no período de carência de uma semana antes de ser desprovisionado.</span><span class="sxs-lookup"><span data-stu-id="34a41-175">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="34a41-176">desprovisionamento</span><span class="sxs-lookup"><span data-stu-id="34a41-176">deprovisioning</span></span>|<span data-ttu-id="34a41-177">O Cloud PC está desprovisionando.</span><span class="sxs-lookup"><span data-stu-id="34a41-177">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="34a41-178">failed</span><span class="sxs-lookup"><span data-stu-id="34a41-178">failed</span></span>|<span data-ttu-id="34a41-179">A operação no Cloud PC falhou.</span><span class="sxs-lookup"><span data-stu-id="34a41-179">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34a41-180">Relações</span><span class="sxs-lookup"><span data-stu-id="34a41-180">Relationships</span></span>

<span data-ttu-id="34a41-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34a41-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34a41-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34a41-182">JSON representation</span></span>

<span data-ttu-id="34a41-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34a41-183">The following is a JSON representation of the resource.</span></span>
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
