---
title: Atualizar deviceHealthScriptRunSummary
description: Atualiza as propriedades de um objeto deviceHealthScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ce21ae48b1bcc6053eb88af38eda4b69d6eccef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235046"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="93794-103">Atualizar deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="93794-103">Update deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="93794-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93794-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93794-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93794-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93794-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93794-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93794-107">Atualiza as propriedades de um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="93794-107">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93794-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93794-108">Prerequisites</span></span>
<span data-ttu-id="93794-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93794-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93794-111">Permission type</span></span>|<span data-ttu-id="93794-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93794-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93794-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93794-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93794-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="93794-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="93794-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93794-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93794-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93794-116">Not supported.</span></span>|
|<span data-ttu-id="93794-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93794-117">Application</span></span>|<span data-ttu-id="93794-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="93794-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93794-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93794-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="93794-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93794-120">Request headers</span></span>
|<span data-ttu-id="93794-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93794-121">Header</span></span>|<span data-ttu-id="93794-122">Valor</span><span class="sxs-lookup"><span data-stu-id="93794-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93794-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93794-123">Authorization</span></span>|<span data-ttu-id="93794-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93794-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93794-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93794-125">Accept</span></span>|<span data-ttu-id="93794-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93794-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93794-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93794-127">Request body</span></span>
<span data-ttu-id="93794-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="93794-128">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="93794-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="93794-129">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="93794-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93794-130">Property</span></span>|<span data-ttu-id="93794-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="93794-131">Type</span></span>|<span data-ttu-id="93794-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="93794-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93794-133">id</span><span class="sxs-lookup"><span data-stu-id="93794-133">id</span></span>|<span data-ttu-id="93794-134">String</span><span class="sxs-lookup"><span data-stu-id="93794-134">String</span></span>|<span data-ttu-id="93794-135">Chave da entidade de Resumo de execução de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93794-135">Key of the device health script run summary entity.</span></span> <span data-ttu-id="93794-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93794-136">This property is read-only.</span></span>|
|<span data-ttu-id="93794-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="93794-138">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-138">Int32</span></span>|<span data-ttu-id="93794-139">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro</span><span class="sxs-lookup"><span data-stu-id="93794-139">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="93794-140">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-140">issueDetectedDeviceCount</span></span>|<span data-ttu-id="93794-141">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-141">Int32</span></span>|<span data-ttu-id="93794-142">Número de dispositivos para os quais o script de detecção encontrou um problema</span><span class="sxs-lookup"><span data-stu-id="93794-142">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="93794-143">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-143">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="93794-144">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-144">Int32</span></span>|<span data-ttu-id="93794-145">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="93794-145">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="93794-146">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-146">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="93794-147">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-147">Int32</span></span>|<span data-ttu-id="93794-148">Número de dispositivos que ainda não executaram a versão mais recente do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="93794-148">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="93794-149">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-149">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="93794-150">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-150">Int32</span></span>|<span data-ttu-id="93794-151">Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="93794-151">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="93794-152">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-152">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="93794-153">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-153">Int32</span></span>|<span data-ttu-id="93794-154">Número de dispositivos para os quais a correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="93794-154">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="93794-155">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-155">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="93794-156">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-156">Int32</span></span>|<span data-ttu-id="93794-157">Número de dispositivos para os quais o script de correção foi executado com êxito, mas falhou ao resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="93794-157">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="93794-158">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-158">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="93794-159">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-159">Int32</span></span>|<span data-ttu-id="93794-160">Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="93794-160">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="93794-161">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="93794-161">lastScriptRunDateTime</span></span>|<span data-ttu-id="93794-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93794-162">DateTimeOffset</span></span>|<span data-ttu-id="93794-163">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="93794-163">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="93794-164">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93794-164">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="93794-165">Int32</span><span class="sxs-lookup"><span data-stu-id="93794-165">Int32</span></span>|<span data-ttu-id="93794-166">Número de dispositivos que foram corrigidos nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="93794-166">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="93794-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="93794-167">Response</span></span>
<span data-ttu-id="93794-168">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93794-168">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93794-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93794-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="93794-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93794-170">Request</span></span>
<span data-ttu-id="93794-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93794-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93794-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="93794-172">Response</span></span>
<span data-ttu-id="93794-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93794-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




