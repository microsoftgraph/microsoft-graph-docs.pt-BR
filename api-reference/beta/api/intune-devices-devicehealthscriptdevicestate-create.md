---
title: Criar deviceHealthScriptDeviceState
description: Crie um novo objeto deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a115878511d7d0317bc17bc38f88538de503b9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130732"
---
# <a name="create-devicehealthscriptdevicestate"></a><span data-ttu-id="3beac-103">Criar deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3beac-103">Create deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="3beac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3beac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3beac-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3beac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3beac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3beac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3beac-107">Crie um novo [objeto deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="3beac-107">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3beac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3beac-108">Prerequisites</span></span>
<span data-ttu-id="3beac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3beac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3beac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3beac-111">Permission type</span></span>|<span data-ttu-id="3beac-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3beac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3beac-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3beac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3beac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3beac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3beac-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3beac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3beac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3beac-116">Not supported.</span></span>|
|<span data-ttu-id="3beac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3beac-117">Application</span></span>|<span data-ttu-id="3beac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3beac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3beac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3beac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="3beac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3beac-120">Request headers</span></span>
|<span data-ttu-id="3beac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3beac-121">Header</span></span>|<span data-ttu-id="3beac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3beac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3beac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3beac-123">Authorization</span></span>|<span data-ttu-id="3beac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3beac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3beac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3beac-125">Accept</span></span>|<span data-ttu-id="3beac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3beac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3beac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3beac-127">Request body</span></span>
<span data-ttu-id="3beac-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceHealthScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="3beac-128">In the request body, supply a JSON representation for the deviceHealthScriptDeviceState object.</span></span>

<span data-ttu-id="3beac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="3beac-129">The following table shows the properties that are required when you create the deviceHealthScriptDeviceState.</span></span>

|<span data-ttu-id="3beac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3beac-130">Property</span></span>|<span data-ttu-id="3beac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3beac-131">Type</span></span>|<span data-ttu-id="3beac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3beac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3beac-133">id</span><span class="sxs-lookup"><span data-stu-id="3beac-133">id</span></span>|<span data-ttu-id="3beac-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3beac-134">String</span></span>|<span data-ttu-id="3beac-135">Chave da entidade de estado do dispositivo de script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3beac-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="3beac-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3beac-136">This property is read-only.</span></span>|
|<span data-ttu-id="3beac-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="3beac-137">detectionState</span></span>|[<span data-ttu-id="3beac-138">runState</span><span class="sxs-lookup"><span data-stu-id="3beac-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="3beac-139">Estado de detecção da última execução de script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3beac-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="3beac-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="3beac-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="3beac-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3beac-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="3beac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3beac-142">DateTimeOffset</span></span>|<span data-ttu-id="3beac-143">O último período de data/hora de quando o script de saúde do dispositivo foi executado</span><span class="sxs-lookup"><span data-stu-id="3beac-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="3beac-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3beac-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="3beac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3beac-145">DateTimeOffset</span></span>|<span data-ttu-id="3beac-146">O próximo horário de quando o script de saúde do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="3beac-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="3beac-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3beac-147">lastSyncDateTime</span></span>|<span data-ttu-id="3beac-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3beac-148">DateTimeOffset</span></span>|<span data-ttu-id="3beac-149">A última vez que a Extensão de Managment do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="3beac-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="3beac-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="3beac-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="3beac-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3beac-151">String</span></span>|<span data-ttu-id="3beac-152">Saída do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="3beac-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="3beac-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="3beac-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="3beac-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3beac-154">String</span></span>|<span data-ttu-id="3beac-155">Erro do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="3beac-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="3beac-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="3beac-156">remediationScriptError</span></span>|<span data-ttu-id="3beac-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3beac-157">String</span></span>|<span data-ttu-id="3beac-158">Saída de erro do script de correção</span><span class="sxs-lookup"><span data-stu-id="3beac-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="3beac-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="3beac-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="3beac-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3beac-160">String</span></span>|<span data-ttu-id="3beac-161">Saída de script de detecção após correção</span><span class="sxs-lookup"><span data-stu-id="3beac-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="3beac-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="3beac-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="3beac-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3beac-163">String</span></span>|<span data-ttu-id="3beac-164">Erro do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="3beac-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="3beac-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="3beac-165">remediationState</span></span>|[<span data-ttu-id="3beac-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="3beac-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="3beac-167">Estado de correção da última execução do script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3beac-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="3beac-168">Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="3beac-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="3beac-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="3beac-169">Response</span></span>
<span data-ttu-id="3beac-170">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3beac-170">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3beac-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3beac-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3beac-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3beac-172">Request</span></span>
<span data-ttu-id="3beac-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3beac-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3beac-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="3beac-174">Response</span></span>
<span data-ttu-id="3beac-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3beac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




