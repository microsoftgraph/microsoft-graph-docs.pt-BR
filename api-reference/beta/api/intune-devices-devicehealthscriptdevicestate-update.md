---
title: Atualizar deviceHealthScriptDeviceState
description: Atualize as propriedades de um objeto deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2520d476265ee9745efa6a017d8de23a2bc77ad
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51609490"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="dde35-103">Atualizar deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="dde35-103">Update deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="dde35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dde35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dde35-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dde35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dde35-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dde35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dde35-107">Atualize as propriedades de [um objeto deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="dde35-107">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dde35-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dde35-108">Prerequisites</span></span>
<span data-ttu-id="dde35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dde35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dde35-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dde35-111">Permission type</span></span>|<span data-ttu-id="dde35-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dde35-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dde35-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dde35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dde35-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dde35-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dde35-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dde35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dde35-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dde35-116">Not supported.</span></span>|
|<span data-ttu-id="dde35-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dde35-117">Application</span></span>|<span data-ttu-id="dde35-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dde35-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dde35-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dde35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="dde35-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dde35-120">Request headers</span></span>
|<span data-ttu-id="dde35-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dde35-121">Header</span></span>|<span data-ttu-id="dde35-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dde35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dde35-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dde35-123">Authorization</span></span>|<span data-ttu-id="dde35-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dde35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dde35-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dde35-125">Accept</span></span>|<span data-ttu-id="dde35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dde35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dde35-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dde35-127">Request body</span></span>
<span data-ttu-id="dde35-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="dde35-128">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="dde35-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="dde35-129">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="dde35-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dde35-130">Property</span></span>|<span data-ttu-id="dde35-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dde35-131">Type</span></span>|<span data-ttu-id="dde35-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dde35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dde35-133">id</span><span class="sxs-lookup"><span data-stu-id="dde35-133">id</span></span>|<span data-ttu-id="dde35-134">String</span><span class="sxs-lookup"><span data-stu-id="dde35-134">String</span></span>|<span data-ttu-id="dde35-135">Chave da entidade de estado do dispositivo de script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dde35-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="dde35-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dde35-136">This property is read-only.</span></span>|
|<span data-ttu-id="dde35-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="dde35-137">detectionState</span></span>|[<span data-ttu-id="dde35-138">runState</span><span class="sxs-lookup"><span data-stu-id="dde35-138">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="dde35-139">Estado de detecção da última execução de script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dde35-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="dde35-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="dde35-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="dde35-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="dde35-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="dde35-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dde35-142">DateTimeOffset</span></span>|<span data-ttu-id="dde35-143">O último período de data/hora de quando o script de saúde do dispositivo foi executado</span><span class="sxs-lookup"><span data-stu-id="dde35-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="dde35-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="dde35-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="dde35-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dde35-145">DateTimeOffset</span></span>|<span data-ttu-id="dde35-146">O próximo horário de quando o script de saúde do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="dde35-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="dde35-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dde35-147">lastSyncDateTime</span></span>|<span data-ttu-id="dde35-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dde35-148">DateTimeOffset</span></span>|<span data-ttu-id="dde35-149">A última vez que a Extensão de Managment do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="dde35-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="dde35-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="dde35-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="dde35-151">String</span><span class="sxs-lookup"><span data-stu-id="dde35-151">String</span></span>|<span data-ttu-id="dde35-152">Saída do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="dde35-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="dde35-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="dde35-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="dde35-154">String</span><span class="sxs-lookup"><span data-stu-id="dde35-154">String</span></span>|<span data-ttu-id="dde35-155">Erro do script de detecção antes da correção</span><span class="sxs-lookup"><span data-stu-id="dde35-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="dde35-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="dde35-156">remediationScriptError</span></span>|<span data-ttu-id="dde35-157">String</span><span class="sxs-lookup"><span data-stu-id="dde35-157">String</span></span>|<span data-ttu-id="dde35-158">Saída de erro do script de correção</span><span class="sxs-lookup"><span data-stu-id="dde35-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="dde35-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="dde35-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="dde35-160">String</span><span class="sxs-lookup"><span data-stu-id="dde35-160">String</span></span>|<span data-ttu-id="dde35-161">Saída de script de detecção após correção</span><span class="sxs-lookup"><span data-stu-id="dde35-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="dde35-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="dde35-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="dde35-163">String</span><span class="sxs-lookup"><span data-stu-id="dde35-163">String</span></span>|<span data-ttu-id="dde35-164">Erro do script de detecção após a correção</span><span class="sxs-lookup"><span data-stu-id="dde35-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="dde35-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="dde35-165">remediationState</span></span>|[<span data-ttu-id="dde35-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="dde35-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="dde35-167">Estado de correção da última execução do script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dde35-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="dde35-168">Os valores possíveis são: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="dde35-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="dde35-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="dde35-169">Response</span></span>
<span data-ttu-id="dde35-170">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dde35-170">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dde35-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dde35-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="dde35-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dde35-172">Request</span></span>
<span data-ttu-id="dde35-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dde35-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dde35-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="dde35-174">Response</span></span>
<span data-ttu-id="dde35-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dde35-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




