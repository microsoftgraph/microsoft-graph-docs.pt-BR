---
title: tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas pela nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d1109ceb81f741cefa9b26662bc1c8c5de8a8329
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563825"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="498cb-103">tipo de recurso cloudPC</span><span class="sxs-lookup"><span data-stu-id="498cb-103">cloudPC resource type</span></span>

<span data-ttu-id="498cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="498cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="498cb-105">Representa uma área de trabalho virtual gerenciada em nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="498cb-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="498cb-106">Methods</span></span>

|<span data-ttu-id="498cb-107">Método</span><span class="sxs-lookup"><span data-stu-id="498cb-107">Method</span></span>|<span data-ttu-id="498cb-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="498cb-108">Return type</span></span>|<span data-ttu-id="498cb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="498cb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="498cb-110">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="498cb-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="498cb-111">coleção [cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="498cb-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="498cb-112">Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="498cb-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="498cb-113">Obter cloudPC</span><span class="sxs-lookup"><span data-stu-id="498cb-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="498cb-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="498cb-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="498cb-115">Leia as propriedades e os relacionamentos de um objeto [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="498cb-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="498cb-116">Reprovisionar</span><span class="sxs-lookup"><span data-stu-id="498cb-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="498cb-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="498cb-117">None</span></span>|<span data-ttu-id="498cb-118">Reprovisionar um objeto [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="498cb-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="498cb-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="498cb-119">Properties</span></span>

|<span data-ttu-id="498cb-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="498cb-120">Property</span></span>|<span data-ttu-id="498cb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="498cb-121">Type</span></span>|<span data-ttu-id="498cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="498cb-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="498cb-123">id</span><span class="sxs-lookup"><span data-stu-id="498cb-123">id</span></span>|<span data-ttu-id="498cb-124">String</span><span class="sxs-lookup"><span data-stu-id="498cb-124">String</span></span>|<span data-ttu-id="498cb-125">Identificador exclusivo do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="498cb-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="498cb-126">Read-only.</span></span>|
|<span data-ttu-id="498cb-127">displayName</span><span class="sxs-lookup"><span data-stu-id="498cb-127">displayName</span></span>|<span data-ttu-id="498cb-128">String</span><span class="sxs-lookup"><span data-stu-id="498cb-128">String</span></span>|<span data-ttu-id="498cb-129">O nome de exibição do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="498cb-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="498cb-130">imageDisplayName</span></span>|<span data-ttu-id="498cb-131">String</span><span class="sxs-lookup"><span data-stu-id="498cb-131">String</span></span>|<span data-ttu-id="498cb-132">Nome da imagem do sistema operacional que está no computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="498cb-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="498cb-133">managedDeviceId</span></span>|<span data-ttu-id="498cb-134">String</span><span class="sxs-lookup"><span data-stu-id="498cb-134">String</span></span>|<span data-ttu-id="498cb-135">A ID de dispositivo do Intune do PC na nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="498cb-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="498cb-136">managedDeviceName</span></span>|<span data-ttu-id="498cb-137">String</span><span class="sxs-lookup"><span data-stu-id="498cb-137">String</span></span>|<span data-ttu-id="498cb-138">O nome do dispositivo do Intune no Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="498cb-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="498cb-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="498cb-139">provisioningPolicyId</span></span>|<span data-ttu-id="498cb-140">String</span><span class="sxs-lookup"><span data-stu-id="498cb-140">String</span></span>|<span data-ttu-id="498cb-141">A ID da política de provisionamento do PC da nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="498cb-142">onplanid</span><span class="sxs-lookup"><span data-stu-id="498cb-142">servicePlanId</span></span>|<span data-ttu-id="498cb-143">String</span><span class="sxs-lookup"><span data-stu-id="498cb-143">String</span></span>|<span data-ttu-id="498cb-144">A ID do plano de serviço do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="498cb-145">onplanname</span><span class="sxs-lookup"><span data-stu-id="498cb-145">servicePlanName</span></span>|<span data-ttu-id="498cb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="498cb-146">String</span></span>|<span data-ttu-id="498cb-147">O nome do plano de serviço do computador da nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="498cb-148">status</span><span class="sxs-lookup"><span data-stu-id="498cb-148">status</span></span>|<span data-ttu-id="498cb-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="498cb-149">cloudPcStatus</span></span>|<span data-ttu-id="498cb-150">Status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-150">Status of the cloud PC.</span></span> <span data-ttu-id="498cb-151">Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.</span><span class="sxs-lookup"><span data-stu-id="498cb-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.</span></span>|
|<span data-ttu-id="498cb-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="498cb-152">statusDetails</span></span>|[<span data-ttu-id="498cb-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="498cb-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="498cb-154">Os detalhes do status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="498cb-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="498cb-155">userPrincipalName</span></span>|<span data-ttu-id="498cb-156">String</span><span class="sxs-lookup"><span data-stu-id="498cb-156">String</span></span>|<span data-ttu-id="498cb-157">O nome principal do usuário (UPN) do usuário atribuído ao computador da nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="498cb-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="498cb-158">lastModifiedDateTime</span></span>|<span data-ttu-id="498cb-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="498cb-159">DateTimeOffset</span></span>|<span data-ttu-id="498cb-160">A data e a hora da última modificação do computador da nuvem.</span><span class="sxs-lookup"><span data-stu-id="498cb-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="498cb-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="498cb-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="498cb-162">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="498cb-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="498cb-163">Relações</span><span class="sxs-lookup"><span data-stu-id="498cb-163">Relationships</span></span>

<span data-ttu-id="498cb-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="498cb-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="498cb-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="498cb-165">JSON representation</span></span>

<span data-ttu-id="498cb-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="498cb-166">The following is a JSON representation of the resource.</span></span>
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
