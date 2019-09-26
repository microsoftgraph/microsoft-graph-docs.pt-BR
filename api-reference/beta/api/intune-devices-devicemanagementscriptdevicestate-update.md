---
title: Atualizar deviceManagementScriptDeviceState
description: Atualiza as propriedades de um objeto deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bfb1dc79bd1162b2b05ddff35c3ea712db3ea97
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188553"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="eb74b-103">Atualizar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="eb74b-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="eb74b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb74b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb74b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb74b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb74b-106">Atualiza as propriedades de um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="eb74b-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb74b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb74b-107">Prerequisites</span></span>
<span data-ttu-id="eb74b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb74b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb74b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb74b-110">Permission type</span></span>|<span data-ttu-id="eb74b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb74b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb74b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb74b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb74b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb74b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="eb74b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb74b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb74b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb74b-115">Not supported.</span></span>|
|<span data-ttu-id="eb74b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb74b-116">Application</span></span>|<span data-ttu-id="eb74b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb74b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb74b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb74b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="eb74b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb74b-119">Request headers</span></span>
|<span data-ttu-id="eb74b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb74b-120">Header</span></span>|<span data-ttu-id="eb74b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb74b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb74b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb74b-122">Authorization</span></span>|<span data-ttu-id="eb74b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb74b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb74b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb74b-124">Accept</span></span>|<span data-ttu-id="eb74b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb74b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb74b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb74b-126">Request body</span></span>
<span data-ttu-id="eb74b-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="eb74b-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="eb74b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="eb74b-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="eb74b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb74b-129">Property</span></span>|<span data-ttu-id="eb74b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb74b-130">Type</span></span>|<span data-ttu-id="eb74b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb74b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb74b-132">id</span><span class="sxs-lookup"><span data-stu-id="eb74b-132">id</span></span>|<span data-ttu-id="eb74b-133">String</span><span class="sxs-lookup"><span data-stu-id="eb74b-133">String</span></span>|<span data-ttu-id="eb74b-134">Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="eb74b-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="eb74b-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb74b-135">This property is read-only.</span></span>|
|<span data-ttu-id="eb74b-136">runState</span><span class="sxs-lookup"><span data-stu-id="eb74b-136">runState</span></span>|[<span data-ttu-id="eb74b-137">runState</span><span class="sxs-lookup"><span data-stu-id="eb74b-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="eb74b-138">Estado da última execução do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="eb74b-138">State of latest run of the device management script.</span></span> <span data-ttu-id="eb74b-139">Os valores possíveis são: `unknown`, `success`, `fail`, `error`, `pending`.</span><span class="sxs-lookup"><span data-stu-id="eb74b-139">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="eb74b-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="eb74b-140">resultMessage</span></span>|<span data-ttu-id="eb74b-141">String</span><span class="sxs-lookup"><span data-stu-id="eb74b-141">String</span></span>|<span data-ttu-id="eb74b-142">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="eb74b-142">Details of execution output.</span></span>|
|<span data-ttu-id="eb74b-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="eb74b-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="eb74b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb74b-144">DateTimeOffset</span></span>|<span data-ttu-id="eb74b-145">Última vez em que o script de gerenciamento de dispositivos é executado.</span><span class="sxs-lookup"><span data-stu-id="eb74b-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="eb74b-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="eb74b-146">errorCode</span></span>|<span data-ttu-id="eb74b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="eb74b-147">Int32</span></span>|<span data-ttu-id="eb74b-148">Código de erro correspondente à execução errada do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="eb74b-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="eb74b-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="eb74b-149">errorDescription</span></span>|<span data-ttu-id="eb74b-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb74b-150">String</span></span>|<span data-ttu-id="eb74b-151">Descrição do erro correspondente à execução errada do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb74b-151">Error description corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="eb74b-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="eb74b-152">lastSyncDateTime</span></span>|<span data-ttu-id="eb74b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb74b-153">DateTimeOffset</span></span>|<span data-ttu-id="eb74b-154">A última vez em que a extensão de gerenciamento do Intune é sincronizada com o Intune.</span><span class="sxs-lookup"><span data-stu-id="eb74b-154">The latest time that Intune Managment Extension syncs to Intune.</span></span>|
|<span data-ttu-id="eb74b-155">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="eb74b-155">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="eb74b-156">String</span><span class="sxs-lookup"><span data-stu-id="eb74b-156">String</span></span>|<span data-ttu-id="eb74b-157">Saída do script de detecção antes da correção.</span><span class="sxs-lookup"><span data-stu-id="eb74b-157">Output of the detection script before remediation.</span></span>|
|<span data-ttu-id="eb74b-158">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="eb74b-158">remediationScriptError</span></span>|<span data-ttu-id="eb74b-159">String</span><span class="sxs-lookup"><span data-stu-id="eb74b-159">String</span></span>|<span data-ttu-id="eb74b-160">Erro de saída do script de correção.</span><span class="sxs-lookup"><span data-stu-id="eb74b-160">Error output of the remediation script.</span></span>|
|<span data-ttu-id="eb74b-161">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="eb74b-161">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="eb74b-162">String</span><span class="sxs-lookup"><span data-stu-id="eb74b-162">String</span></span>|<span data-ttu-id="eb74b-163">A saída do script de detecção após a correção.</span><span class="sxs-lookup"><span data-stu-id="eb74b-163">Detection script output after remediation.</span></span>|



## <a name="response"></a><span data-ttu-id="eb74b-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb74b-164">Response</span></span>
<span data-ttu-id="eb74b-165">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb74b-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb74b-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb74b-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb74b-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb74b-167">Request</span></span>
<span data-ttu-id="eb74b-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb74b-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
}
```

### <a name="response"></a><span data-ttu-id="eb74b-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb74b-169">Response</span></span>
<span data-ttu-id="eb74b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb74b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
}
```




