---
title: Atualizar deviceHealthScriptDeviceState
description: Atualiza as propriedades de um objeto deviceHealthScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3899f1ae9d0860ee2eca169169bb9012358bb886
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945057"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="d2790-103">Atualizar deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="d2790-103">Update deviceHealthScriptDeviceState</span></span>

> <span data-ttu-id="d2790-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2790-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2790-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2790-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2790-106">Atualiza as propriedades de um objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d2790-106">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2790-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2790-107">Prerequisites</span></span>
<span data-ttu-id="d2790-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2790-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2790-110">Permission type</span></span>|<span data-ttu-id="d2790-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2790-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2790-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2790-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2790-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2790-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d2790-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2790-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2790-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2790-115">Not supported.</span></span>|
|<span data-ttu-id="d2790-116">Application</span><span class="sxs-lookup"><span data-stu-id="d2790-116">Application</span></span>|<span data-ttu-id="d2790-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2790-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2790-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2790-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d2790-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2790-119">Request headers</span></span>
|<span data-ttu-id="d2790-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2790-120">Header</span></span>|<span data-ttu-id="d2790-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d2790-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2790-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2790-122">Authorization</span></span>|<span data-ttu-id="d2790-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2790-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2790-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2790-124">Accept</span></span>|<span data-ttu-id="d2790-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2790-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2790-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2790-126">Request body</span></span>
<span data-ttu-id="d2790-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d2790-127">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="d2790-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="d2790-128">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="d2790-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2790-129">Property</span></span>|<span data-ttu-id="d2790-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2790-130">Type</span></span>|<span data-ttu-id="d2790-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2790-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2790-132">id</span><span class="sxs-lookup"><span data-stu-id="d2790-132">id</span></span>|<span data-ttu-id="d2790-133">String</span><span class="sxs-lookup"><span data-stu-id="d2790-133">String</span></span>|<span data-ttu-id="d2790-134">Chave da entidade de estado do dispositivo de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d2790-134">Key of the device health script device state entity.</span></span> <span data-ttu-id="d2790-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2790-135">This property is read-only.</span></span>|
|<span data-ttu-id="d2790-136">detecçaostate</span><span class="sxs-lookup"><span data-stu-id="d2790-136">detectionState</span></span>|[<span data-ttu-id="d2790-137">runState</span><span class="sxs-lookup"><span data-stu-id="d2790-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d2790-138">Estado de detecção da execução do script de integridade do dispositivo mais recente.</span><span class="sxs-lookup"><span data-stu-id="d2790-138">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="d2790-139">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="d2790-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="d2790-140">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d2790-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="d2790-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2790-141">DateTimeOffset</span></span>|<span data-ttu-id="d2790-142">O último carimbo de data/hora de quando o script de integridade do dispositivo é executado</span><span class="sxs-lookup"><span data-stu-id="d2790-142">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="d2790-143">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d2790-143">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="d2790-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2790-144">DateTimeOffset</span></span>|<span data-ttu-id="d2790-145">O carimbo de data/hora seguinte de quando o script de integridade do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="d2790-145">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="d2790-146">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d2790-146">lastSyncDateTime</span></span>|<span data-ttu-id="d2790-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2790-147">DateTimeOffset</span></span>|<span data-ttu-id="d2790-148">A última vez em que a extensão de gerenciamento do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="d2790-148">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="d2790-149">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="d2790-149">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="d2790-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d2790-150">String</span></span>|<span data-ttu-id="d2790-151">Saída do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="d2790-151">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="d2790-152">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="d2790-152">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="d2790-153">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d2790-153">String</span></span>|<span data-ttu-id="d2790-154">Erro do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="d2790-154">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="d2790-155">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="d2790-155">remediationScriptError</span></span>|<span data-ttu-id="d2790-156">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d2790-156">String</span></span>|<span data-ttu-id="d2790-157">Saída de erro do script de correção</span><span class="sxs-lookup"><span data-stu-id="d2790-157">Error output of the remediation script</span></span>|
|<span data-ttu-id="d2790-158">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="d2790-158">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="d2790-159">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d2790-159">String</span></span>|<span data-ttu-id="d2790-160">Saída do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="d2790-160">Detection script output after remediation</span></span>|
|<span data-ttu-id="d2790-161">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="d2790-161">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="d2790-162">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d2790-162">String</span></span>|<span data-ttu-id="d2790-163">Erro do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="d2790-163">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="d2790-164">remediationState</span><span class="sxs-lookup"><span data-stu-id="d2790-164">remediationState</span></span>|[<span data-ttu-id="d2790-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="d2790-165">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="d2790-166">Estado de correção da execução do script de integridade do dispositivo mais recente.</span><span class="sxs-lookup"><span data-stu-id="d2790-166">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="d2790-167">Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="d2790-167">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="d2790-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2790-168">Response</span></span>
<span data-ttu-id="d2790-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2790-169">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2790-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2790-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2790-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2790-171">Request</span></span>
<span data-ttu-id="d2790-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2790-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
Content-type: application/json
Content-length: 762

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```

### <a name="response"></a><span data-ttu-id="d2790-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2790-173">Response</span></span>
<span data-ttu-id="d2790-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2790-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 811

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```





