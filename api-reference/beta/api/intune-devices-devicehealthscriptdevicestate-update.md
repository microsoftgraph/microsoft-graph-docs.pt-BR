---
title: Atualizar deviceHealthScriptDeviceState
description: Atualiza as propriedades de um objeto deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cf7a6cc3ca58317d54326509b658a10b2549fd1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093949"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="37705-103">Atualizar deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="37705-103">Update deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="37705-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37705-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37705-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37705-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37705-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37705-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37705-107">Atualiza as propriedades de um objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="37705-107">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37705-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37705-108">Prerequisites</span></span>
<span data-ttu-id="37705-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37705-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37705-111">Permission type</span></span>|<span data-ttu-id="37705-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37705-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37705-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37705-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37705-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37705-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="37705-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37705-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37705-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37705-116">Not supported.</span></span>|
|<span data-ttu-id="37705-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37705-117">Application</span></span>|<span data-ttu-id="37705-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37705-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37705-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37705-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="37705-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37705-120">Request headers</span></span>
|<span data-ttu-id="37705-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37705-121">Header</span></span>|<span data-ttu-id="37705-122">Valor</span><span class="sxs-lookup"><span data-stu-id="37705-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37705-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37705-123">Authorization</span></span>|<span data-ttu-id="37705-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37705-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37705-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37705-125">Accept</span></span>|<span data-ttu-id="37705-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37705-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37705-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37705-127">Request body</span></span>
<span data-ttu-id="37705-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="37705-128">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="37705-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="37705-129">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="37705-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37705-130">Property</span></span>|<span data-ttu-id="37705-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="37705-131">Type</span></span>|<span data-ttu-id="37705-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="37705-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37705-133">id</span><span class="sxs-lookup"><span data-stu-id="37705-133">id</span></span>|<span data-ttu-id="37705-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37705-134">String</span></span>|<span data-ttu-id="37705-135">Chave da entidade de estado do dispositivo de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37705-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="37705-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37705-136">This property is read-only.</span></span>|
|<span data-ttu-id="37705-137">detecçaostate</span><span class="sxs-lookup"><span data-stu-id="37705-137">detectionState</span></span>|[<span data-ttu-id="37705-138">runState</span><span class="sxs-lookup"><span data-stu-id="37705-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="37705-139">Estado de detecção da execução do script de integridade do dispositivo mais recente.</span><span class="sxs-lookup"><span data-stu-id="37705-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="37705-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="37705-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="37705-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="37705-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="37705-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37705-142">DateTimeOffset</span></span>|<span data-ttu-id="37705-143">O último carimbo de data/hora de quando o script de integridade do dispositivo é executado</span><span class="sxs-lookup"><span data-stu-id="37705-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="37705-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="37705-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="37705-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37705-145">DateTimeOffset</span></span>|<span data-ttu-id="37705-146">O carimbo de data/hora seguinte de quando o script de integridade do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="37705-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="37705-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="37705-147">lastSyncDateTime</span></span>|<span data-ttu-id="37705-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37705-148">DateTimeOffset</span></span>|<span data-ttu-id="37705-149">A última vez em que a extensão de gerenciamento do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="37705-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="37705-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="37705-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="37705-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37705-151">String</span></span>|<span data-ttu-id="37705-152">Saída do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="37705-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="37705-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="37705-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="37705-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37705-154">String</span></span>|<span data-ttu-id="37705-155">Erro do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="37705-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="37705-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="37705-156">remediationScriptError</span></span>|<span data-ttu-id="37705-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37705-157">String</span></span>|<span data-ttu-id="37705-158">Saída de erro do script de correção</span><span class="sxs-lookup"><span data-stu-id="37705-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="37705-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="37705-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="37705-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37705-160">String</span></span>|<span data-ttu-id="37705-161">Saída do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="37705-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="37705-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="37705-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="37705-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37705-163">String</span></span>|<span data-ttu-id="37705-164">Erro do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="37705-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="37705-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="37705-165">remediationState</span></span>|[<span data-ttu-id="37705-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="37705-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="37705-167">Estado de correção da execução do script de integridade do dispositivo mais recente.</span><span class="sxs-lookup"><span data-stu-id="37705-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="37705-168">Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="37705-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="37705-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="37705-169">Response</span></span>
<span data-ttu-id="37705-170">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37705-170">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37705-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37705-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="37705-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37705-172">Request</span></span>
<span data-ttu-id="37705-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37705-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37705-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="37705-174">Response</span></span>
<span data-ttu-id="37705-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37705-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






