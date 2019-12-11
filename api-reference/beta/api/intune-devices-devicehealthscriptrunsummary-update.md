---
title: Atualizar deviceHealthScriptRunSummary
description: Atualiza as propriedades de um objeto deviceHealthScriptRunSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a102b6624a2bedf70708ac4fedb03c523c34511
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945036"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="fce0f-103">Atualizar deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="fce0f-103">Update deviceHealthScriptRunSummary</span></span>

> <span data-ttu-id="fce0f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fce0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fce0f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fce0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fce0f-106">Atualiza as propriedades de um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="fce0f-106">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fce0f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fce0f-107">Prerequisites</span></span>
<span data-ttu-id="fce0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fce0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fce0f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fce0f-110">Permission type</span></span>|<span data-ttu-id="fce0f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fce0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fce0f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fce0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fce0f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce0f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fce0f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fce0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fce0f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fce0f-115">Not supported.</span></span>|
|<span data-ttu-id="fce0f-116">Application</span><span class="sxs-lookup"><span data-stu-id="fce0f-116">Application</span></span>|<span data-ttu-id="fce0f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce0f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fce0f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fce0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="fce0f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fce0f-119">Request headers</span></span>
|<span data-ttu-id="fce0f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fce0f-120">Header</span></span>|<span data-ttu-id="fce0f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fce0f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fce0f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fce0f-122">Authorization</span></span>|<span data-ttu-id="fce0f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fce0f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fce0f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fce0f-124">Accept</span></span>|<span data-ttu-id="fce0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fce0f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fce0f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fce0f-126">Request body</span></span>
<span data-ttu-id="fce0f-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="fce0f-127">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="fce0f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="fce0f-128">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="fce0f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fce0f-129">Property</span></span>|<span data-ttu-id="fce0f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fce0f-130">Type</span></span>|<span data-ttu-id="fce0f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fce0f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce0f-132">id</span><span class="sxs-lookup"><span data-stu-id="fce0f-132">id</span></span>|<span data-ttu-id="fce0f-133">String</span><span class="sxs-lookup"><span data-stu-id="fce0f-133">String</span></span>|<span data-ttu-id="fce0f-134">Chave da entidade de Resumo de execução de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce0f-134">Key of the device health script run summary entity.</span></span> <span data-ttu-id="fce0f-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fce0f-135">This property is read-only.</span></span>|
|<span data-ttu-id="fce0f-136">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-136">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="fce0f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-137">Int32</span></span>|<span data-ttu-id="fce0f-138">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro</span><span class="sxs-lookup"><span data-stu-id="fce0f-138">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="fce0f-139">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-139">issueDetectedDeviceCount</span></span>|<span data-ttu-id="fce0f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-140">Int32</span></span>|<span data-ttu-id="fce0f-141">Número de dispositivos para os quais o script de detecção encontrou um problema</span><span class="sxs-lookup"><span data-stu-id="fce0f-141">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="fce0f-142">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-142">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="fce0f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-143">Int32</span></span>|<span data-ttu-id="fce0f-144">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="fce0f-144">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="fce0f-145">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-145">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="fce0f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-146">Int32</span></span>|<span data-ttu-id="fce0f-147">Número de dispositivos que ainda não executaram a versão mais recente do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="fce0f-147">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="fce0f-148">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-148">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="fce0f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-149">Int32</span></span>|<span data-ttu-id="fce0f-150">Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="fce0f-150">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="fce0f-151">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-151">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="fce0f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-152">Int32</span></span>|<span data-ttu-id="fce0f-153">Número de dispositivos para os quais a correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="fce0f-153">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="fce0f-154">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-154">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="fce0f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-155">Int32</span></span>|<span data-ttu-id="fce0f-156">Número de dispositivos para os quais o script de correção foi executado com êxito, mas falhou ao resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="fce0f-156">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="fce0f-157">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-157">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="fce0f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-158">Int32</span></span>|<span data-ttu-id="fce0f-159">Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="fce0f-159">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="fce0f-160">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="fce0f-160">lastScriptRunDateTime</span></span>|<span data-ttu-id="fce0f-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fce0f-161">DateTimeOffset</span></span>|<span data-ttu-id="fce0f-162">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="fce0f-162">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="fce0f-163">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fce0f-163">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="fce0f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fce0f-164">Int32</span></span>|<span data-ttu-id="fce0f-165">Número de dispositivos que foram corrigidos nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="fce0f-165">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="fce0f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce0f-166">Response</span></span>
<span data-ttu-id="fce0f-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fce0f-167">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fce0f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fce0f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="fce0f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fce0f-169">Request</span></span>
<span data-ttu-id="fce0f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fce0f-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a><span data-ttu-id="fce0f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce0f-171">Response</span></span>
<span data-ttu-id="fce0f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fce0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```





