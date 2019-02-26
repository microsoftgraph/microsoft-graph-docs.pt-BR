---
title: Atualizar deviceComplianceDeviceOverview
description: Atualizar as propriedades de um objeto deviceComplianceDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d09535f2309370984834d150c8aa55cbe436256
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174365"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="d6317-103">Atualizar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d6317-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="d6317-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6317-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6317-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6317-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6317-106">Atualizar as propriedades de um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d6317-106">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6317-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6317-107">Prerequisites</span></span>
<span data-ttu-id="d6317-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d6317-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6317-110">Permission type</span></span>|<span data-ttu-id="d6317-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6317-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6317-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6317-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6317-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6317-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6317-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6317-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6317-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6317-115">Not supported.</span></span>|
|<span data-ttu-id="d6317-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6317-116">Application</span></span>|<span data-ttu-id="d6317-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6317-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6317-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6317-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="d6317-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6317-119">Request headers</span></span>
|<span data-ttu-id="d6317-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6317-120">Header</span></span>|<span data-ttu-id="d6317-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d6317-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6317-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6317-122">Authorization</span></span>|<span data-ttu-id="d6317-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6317-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6317-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6317-124">Accept</span></span>|<span data-ttu-id="d6317-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6317-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6317-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6317-126">Request body</span></span>
<span data-ttu-id="d6317-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d6317-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="d6317-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="d6317-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="d6317-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6317-129">Property</span></span>|<span data-ttu-id="d6317-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6317-130">Type</span></span>|<span data-ttu-id="d6317-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6317-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6317-132">id</span><span class="sxs-lookup"><span data-stu-id="d6317-132">id</span></span>|<span data-ttu-id="d6317-133">String</span><span class="sxs-lookup"><span data-stu-id="d6317-133">String</span></span>|<span data-ttu-id="d6317-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6317-134">Key of the entity.</span></span>|
|<span data-ttu-id="d6317-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d6317-135">pendingCount</span></span>|<span data-ttu-id="d6317-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-136">Int32</span></span>|<span data-ttu-id="d6317-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="d6317-137">Number of pending devices</span></span>|
|<span data-ttu-id="d6317-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d6317-138">notApplicableCount</span></span>|<span data-ttu-id="d6317-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-139">Int32</span></span>|<span data-ttu-id="d6317-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="d6317-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="d6317-141">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="d6317-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="d6317-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-142">Int32</span></span>|<span data-ttu-id="d6317-143">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="d6317-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="d6317-144">successCount</span><span class="sxs-lookup"><span data-stu-id="d6317-144">successCount</span></span>|<span data-ttu-id="d6317-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-145">Int32</span></span>|<span data-ttu-id="d6317-146">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="d6317-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="d6317-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="d6317-147">errorCount</span></span>|<span data-ttu-id="d6317-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-148">Int32</span></span>|<span data-ttu-id="d6317-149">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="d6317-149">Number of error devices</span></span>|
|<span data-ttu-id="d6317-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="d6317-150">failedCount</span></span>|<span data-ttu-id="d6317-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-151">Int32</span></span>|<span data-ttu-id="d6317-152">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="d6317-152">Number of failed devices</span></span>|
|<span data-ttu-id="d6317-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d6317-153">conflictCount</span></span>|<span data-ttu-id="d6317-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-154">Int32</span></span>|<span data-ttu-id="d6317-155">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="d6317-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="d6317-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d6317-156">lastUpdateDateTime</span></span>|<span data-ttu-id="d6317-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6317-157">DateTimeOffset</span></span>|<span data-ttu-id="d6317-158">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="d6317-158">Last update time</span></span>|
|<span data-ttu-id="d6317-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d6317-159">configurationVersion</span></span>|<span data-ttu-id="d6317-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d6317-160">Int32</span></span>|<span data-ttu-id="d6317-161">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="d6317-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="d6317-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6317-162">Response</span></span>
<span data-ttu-id="d6317-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6317-163">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6317-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6317-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6317-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6317-165">Request</span></span>
<span data-ttu-id="d6317-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6317-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="d6317-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6317-167">Response</span></span>
<span data-ttu-id="d6317-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6317-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




