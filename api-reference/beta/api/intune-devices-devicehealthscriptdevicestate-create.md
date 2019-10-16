---
title: Criar deviceHealthScriptDeviceState
description: Criar um novo objeto deviceHealthScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ad913ac849ecccd4fd2856d70210f56c120b6fe
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531403"
---
# <a name="create-devicehealthscriptdevicestate"></a><span data-ttu-id="4ac94-103">Criar deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4ac94-103">Create deviceHealthScriptDeviceState</span></span>

> <span data-ttu-id="4ac94-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ac94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ac94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ac94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ac94-106">Criar um novo objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="4ac94-106">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ac94-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ac94-107">Prerequisites</span></span>
<span data-ttu-id="4ac94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ac94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ac94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ac94-110">Permission type</span></span>|<span data-ttu-id="4ac94-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ac94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ac94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ac94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ac94-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ac94-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4ac94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ac94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ac94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ac94-115">Not supported.</span></span>|
|<span data-ttu-id="4ac94-116">Application</span><span class="sxs-lookup"><span data-stu-id="4ac94-116">Application</span></span>|<span data-ttu-id="4ac94-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ac94-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ac94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ac94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="4ac94-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ac94-119">Request headers</span></span>
|<span data-ttu-id="4ac94-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ac94-120">Header</span></span>|<span data-ttu-id="4ac94-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4ac94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ac94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ac94-122">Authorization</span></span>|<span data-ttu-id="4ac94-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ac94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ac94-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ac94-124">Accept</span></span>|<span data-ttu-id="4ac94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ac94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ac94-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ac94-126">Request body</span></span>
<span data-ttu-id="4ac94-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="4ac94-127">In the request body, supply a JSON representation for the deviceHealthScriptDeviceState object.</span></span>

<span data-ttu-id="4ac94-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="4ac94-128">The following table shows the properties that are required when you create the deviceHealthScriptDeviceState.</span></span>

|<span data-ttu-id="4ac94-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ac94-129">Property</span></span>|<span data-ttu-id="4ac94-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ac94-130">Type</span></span>|<span data-ttu-id="4ac94-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ac94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ac94-132">id</span><span class="sxs-lookup"><span data-stu-id="4ac94-132">id</span></span>|<span data-ttu-id="4ac94-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ac94-133">String</span></span>|<span data-ttu-id="4ac94-134">Chave da entidade de estado do dispositivo de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ac94-134">Key of the device health script device state entity.</span></span> <span data-ttu-id="4ac94-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4ac94-135">This property is read-only.</span></span>|
|<span data-ttu-id="4ac94-136">detecçaostate</span><span class="sxs-lookup"><span data-stu-id="4ac94-136">detectionState</span></span>|[<span data-ttu-id="4ac94-137">runState</span><span class="sxs-lookup"><span data-stu-id="4ac94-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4ac94-138">Estado de detecção da execução do script de integridade do dispositivo mais recente.</span><span class="sxs-lookup"><span data-stu-id="4ac94-138">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="4ac94-139">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="4ac94-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="4ac94-140">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4ac94-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="4ac94-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ac94-141">DateTimeOffset</span></span>|<span data-ttu-id="4ac94-142">O último carimbo de data/hora de quando o script de integridade do dispositivo é executado</span><span class="sxs-lookup"><span data-stu-id="4ac94-142">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="4ac94-143">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4ac94-143">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="4ac94-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ac94-144">DateTimeOffset</span></span>|<span data-ttu-id="4ac94-145">O carimbo de data/hora seguinte de quando o script de integridade do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="4ac94-145">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="4ac94-146">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4ac94-146">lastSyncDateTime</span></span>|<span data-ttu-id="4ac94-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ac94-147">DateTimeOffset</span></span>|<span data-ttu-id="4ac94-148">A última vez em que a extensão de gerenciamento do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="4ac94-148">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="4ac94-149">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="4ac94-149">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="4ac94-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ac94-150">String</span></span>|<span data-ttu-id="4ac94-151">Saída do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="4ac94-151">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="4ac94-152">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="4ac94-152">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="4ac94-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ac94-153">String</span></span>|<span data-ttu-id="4ac94-154">Erro do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="4ac94-154">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="4ac94-155">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="4ac94-155">remediationScriptError</span></span>|<span data-ttu-id="4ac94-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ac94-156">String</span></span>|<span data-ttu-id="4ac94-157">Saída de erro do script de correção</span><span class="sxs-lookup"><span data-stu-id="4ac94-157">Error output of the remediation script</span></span>|
|<span data-ttu-id="4ac94-158">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="4ac94-158">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="4ac94-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ac94-159">String</span></span>|<span data-ttu-id="4ac94-160">Saída do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="4ac94-160">Detection script output after remediation</span></span>|
|<span data-ttu-id="4ac94-161">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="4ac94-161">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="4ac94-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ac94-162">String</span></span>|<span data-ttu-id="4ac94-163">Erro do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="4ac94-163">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="4ac94-164">remediable</span><span class="sxs-lookup"><span data-stu-id="4ac94-164">remediationState</span></span>|[<span data-ttu-id="4ac94-165">remediable</span><span class="sxs-lookup"><span data-stu-id="4ac94-165">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="4ac94-166">Estado de correção da execução do script de integridade do dispositivo mais recente.</span><span class="sxs-lookup"><span data-stu-id="4ac94-166">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="4ac94-167">Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="4ac94-167">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="4ac94-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ac94-168">Response</span></span>
<span data-ttu-id="4ac94-169">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ac94-169">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ac94-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ac94-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ac94-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ac94-171">Request</span></span>
<span data-ttu-id="4ac94-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ac94-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="4ac94-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ac94-173">Response</span></span>
<span data-ttu-id="4ac94-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ac94-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






