---
title: Atualizar deviceHealthScriptRunSummary
description: Atualiza as propriedades de um objeto deviceHealthScriptRunSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1f56c3f379db209ec1bef61a580e9d729ea5012
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768895"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="d3365-103">Atualizar deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d3365-103">Update deviceHealthScriptRunSummary</span></span>

> <span data-ttu-id="d3365-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3365-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3365-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3365-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3365-106">Atualiza as propriedades de um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d3365-106">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3365-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3365-107">Prerequisites</span></span>
<span data-ttu-id="d3365-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3365-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3365-110">Permission type</span></span>|<span data-ttu-id="d3365-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3365-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3365-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3365-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3365-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3365-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d3365-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3365-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3365-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3365-115">Not supported.</span></span>|
|<span data-ttu-id="d3365-116">Application</span><span class="sxs-lookup"><span data-stu-id="d3365-116">Application</span></span>|<span data-ttu-id="d3365-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3365-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3365-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3365-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="d3365-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3365-119">Request headers</span></span>
|<span data-ttu-id="d3365-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3365-120">Header</span></span>|<span data-ttu-id="d3365-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d3365-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3365-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3365-122">Authorization</span></span>|<span data-ttu-id="d3365-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3365-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3365-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3365-124">Accept</span></span>|<span data-ttu-id="d3365-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3365-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3365-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3365-126">Request body</span></span>
<span data-ttu-id="d3365-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d3365-127">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="d3365-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d3365-128">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="d3365-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3365-129">Property</span></span>|<span data-ttu-id="d3365-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3365-130">Type</span></span>|<span data-ttu-id="d3365-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3365-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3365-132">id</span><span class="sxs-lookup"><span data-stu-id="d3365-132">id</span></span>|<span data-ttu-id="d3365-133">String</span><span class="sxs-lookup"><span data-stu-id="d3365-133">String</span></span>|<span data-ttu-id="d3365-134">Chave da entidade de Resumo de execução de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3365-134">Key of the device health script run summary entity.</span></span> <span data-ttu-id="d3365-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3365-135">This property is read-only.</span></span>|
|<span data-ttu-id="d3365-136">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-136">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="d3365-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-137">Int32</span></span>|<span data-ttu-id="d3365-138">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro</span><span class="sxs-lookup"><span data-stu-id="d3365-138">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="d3365-139">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-139">issueDetectedDeviceCount</span></span>|<span data-ttu-id="d3365-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-140">Int32</span></span>|<span data-ttu-id="d3365-141">Número de dispositivos para os quais o script de detecção encontrou um problema</span><span class="sxs-lookup"><span data-stu-id="d3365-141">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="d3365-142">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-142">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="d3365-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-143">Int32</span></span>|<span data-ttu-id="d3365-144">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="d3365-144">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="d3365-145">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-145">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="d3365-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-146">Int32</span></span>|<span data-ttu-id="d3365-147">Número de dispositivos que ainda não executaram a versão mais recente do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3365-147">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="d3365-148">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-148">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="d3365-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-149">Int32</span></span>|<span data-ttu-id="d3365-150">Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="d3365-150">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="d3365-151">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-151">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="d3365-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-152">Int32</span></span>|<span data-ttu-id="d3365-153">Número de dispositivos para os quais a correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="d3365-153">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="d3365-154">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-154">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="d3365-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-155">Int32</span></span>|<span data-ttu-id="d3365-156">Número de dispositivos para os quais o script de correção foi executado com êxito, mas falhou ao resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="d3365-156">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="d3365-157">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-157">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="d3365-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-158">Int32</span></span>|<span data-ttu-id="d3365-159">Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="d3365-159">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="d3365-160">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="d3365-160">lastScriptRunDateTime</span></span>|<span data-ttu-id="d3365-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3365-161">DateTimeOffset</span></span>|<span data-ttu-id="d3365-162">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="d3365-162">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="d3365-163">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3365-163">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="d3365-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d3365-164">Int32</span></span>|<span data-ttu-id="d3365-165">Número de dispositivos que foram corrigidos nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="d3365-165">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="d3365-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3365-166">Response</span></span>
<span data-ttu-id="d3365-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3365-167">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3365-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3365-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3365-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3365-169">Request</span></span>
<span data-ttu-id="d3365-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3365-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3365-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3365-171">Response</span></span>
<span data-ttu-id="d3365-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3365-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




