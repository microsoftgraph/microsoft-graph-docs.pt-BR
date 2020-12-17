---
title: tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas pela nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 481bcae691632685cafab00a4b7e44addb1ad0cd
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706077"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="282e9-103">tipo de recurso cloudPC</span><span class="sxs-lookup"><span data-stu-id="282e9-103">cloudPC resource type</span></span>

<span data-ttu-id="282e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="282e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="282e9-105">Representa uma área de trabalho virtual gerenciada em nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="282e9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="282e9-106">Methods</span></span>

|<span data-ttu-id="282e9-107">Método</span><span class="sxs-lookup"><span data-stu-id="282e9-107">Method</span></span>|<span data-ttu-id="282e9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="282e9-108">Return type</span></span>|<span data-ttu-id="282e9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="282e9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="282e9-110">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="282e9-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="282e9-111">coleção [cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="282e9-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="282e9-112">Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="282e9-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="282e9-113">Obter cloudPC</span><span class="sxs-lookup"><span data-stu-id="282e9-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="282e9-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="282e9-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="282e9-115">Leia as propriedades e os relacionamentos de um objeto [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="282e9-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="282e9-116">Reprovisionar</span><span class="sxs-lookup"><span data-stu-id="282e9-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="282e9-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="282e9-117">None</span></span>|<span data-ttu-id="282e9-118">Reprovisionar um objeto [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="282e9-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="282e9-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="282e9-119">Properties</span></span>

|<span data-ttu-id="282e9-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="282e9-120">Property</span></span>|<span data-ttu-id="282e9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="282e9-121">Type</span></span>|<span data-ttu-id="282e9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="282e9-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="282e9-123">id</span><span class="sxs-lookup"><span data-stu-id="282e9-123">id</span></span>|<span data-ttu-id="282e9-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-124">String</span></span>|<span data-ttu-id="282e9-125">Identificador exclusivo do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="282e9-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="282e9-126">Read-only.</span></span>|
|<span data-ttu-id="282e9-127">displayName</span><span class="sxs-lookup"><span data-stu-id="282e9-127">displayName</span></span>|<span data-ttu-id="282e9-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-128">String</span></span>|<span data-ttu-id="282e9-129">O nome de exibição do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="282e9-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="282e9-130">imageDisplayName</span></span>|<span data-ttu-id="282e9-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-131">String</span></span>|<span data-ttu-id="282e9-132">Nome da imagem do sistema operacional que está no computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="282e9-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="282e9-133">managedDeviceId</span></span>|<span data-ttu-id="282e9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-134">String</span></span>|<span data-ttu-id="282e9-135">A ID de dispositivo do Intune do PC na nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="282e9-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="282e9-136">managedDeviceName</span></span>|<span data-ttu-id="282e9-137">String</span><span class="sxs-lookup"><span data-stu-id="282e9-137">String</span></span>|<span data-ttu-id="282e9-138">O nome do dispositivo do Intune no Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="282e9-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="282e9-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="282e9-139">provisioningPolicyId</span></span>|<span data-ttu-id="282e9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-140">String</span></span>|<span data-ttu-id="282e9-141">A ID da política de provisionamento do PC da nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="282e9-142">onplanid</span><span class="sxs-lookup"><span data-stu-id="282e9-142">servicePlanId</span></span>|<span data-ttu-id="282e9-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-143">String</span></span>|<span data-ttu-id="282e9-144">A ID do plano de serviço do computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="282e9-145">onplanname</span><span class="sxs-lookup"><span data-stu-id="282e9-145">servicePlanName</span></span>|<span data-ttu-id="282e9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-146">String</span></span>|<span data-ttu-id="282e9-147">O nome do plano de serviço do computador da nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="282e9-148">status</span><span class="sxs-lookup"><span data-stu-id="282e9-148">status</span></span>|<span data-ttu-id="282e9-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="282e9-149">cloudPcStatus</span></span>|<span data-ttu-id="282e9-150">Status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-150">Status of the cloud PC.</span></span> <span data-ttu-id="282e9-151">Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="282e9-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="282e9-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="282e9-152">statusDetails</span></span>|[<span data-ttu-id="282e9-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="282e9-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="282e9-154">Os detalhes do status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="282e9-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="282e9-155">userPrincipalName</span></span>|<span data-ttu-id="282e9-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282e9-156">String</span></span>|<span data-ttu-id="282e9-157">O nome principal do usuário (UPN) do usuário atribuído ao computador da nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="282e9-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="282e9-158">lastModifiedDateTime</span></span>|<span data-ttu-id="282e9-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="282e9-159">DateTimeOffset</span></span>|<span data-ttu-id="282e9-160">A data e a hora da última modificação do computador da nuvem.</span><span class="sxs-lookup"><span data-stu-id="282e9-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="282e9-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="282e9-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="282e9-162">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="282e9-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="282e9-163">Relações</span><span class="sxs-lookup"><span data-stu-id="282e9-163">Relationships</span></span>

<span data-ttu-id="282e9-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="282e9-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="282e9-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="282e9-165">JSON representation</span></span>

<span data-ttu-id="282e9-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="282e9-166">The following is a JSON representation of the resource.</span></span>
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
