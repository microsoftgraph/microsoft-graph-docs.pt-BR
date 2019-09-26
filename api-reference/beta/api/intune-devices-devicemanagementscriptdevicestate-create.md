---
title: Criar deviceManagementScriptDeviceState
description: Criar um novo objeto deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f613c6bb7d8a9fa25a9ef6007701433a1c2f799
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188560"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="56611-103">Criar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="56611-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="56611-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56611-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56611-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56611-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56611-106">Criar um novo objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="56611-106">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56611-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56611-107">Prerequisites</span></span>
<span data-ttu-id="56611-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56611-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56611-110">Permission type</span></span>|<span data-ttu-id="56611-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56611-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56611-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56611-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56611-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56611-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56611-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56611-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56611-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56611-115">Not supported.</span></span>|
|<span data-ttu-id="56611-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56611-116">Application</span></span>|<span data-ttu-id="56611-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56611-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56611-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56611-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="56611-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56611-119">Request headers</span></span>
|<span data-ttu-id="56611-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56611-120">Header</span></span>|<span data-ttu-id="56611-121">Valor</span><span class="sxs-lookup"><span data-stu-id="56611-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56611-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="56611-122">Authorization</span></span>|<span data-ttu-id="56611-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56611-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56611-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56611-124">Accept</span></span>|<span data-ttu-id="56611-125">application/json</span><span class="sxs-lookup"><span data-stu-id="56611-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56611-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56611-126">Request body</span></span>
<span data-ttu-id="56611-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="56611-127">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="56611-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="56611-128">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="56611-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56611-129">Property</span></span>|<span data-ttu-id="56611-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="56611-130">Type</span></span>|<span data-ttu-id="56611-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="56611-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56611-132">id</span><span class="sxs-lookup"><span data-stu-id="56611-132">id</span></span>|<span data-ttu-id="56611-133">String</span><span class="sxs-lookup"><span data-stu-id="56611-133">String</span></span>|<span data-ttu-id="56611-134">Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="56611-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="56611-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56611-135">This property is read-only.</span></span>|
|<span data-ttu-id="56611-136">runState</span><span class="sxs-lookup"><span data-stu-id="56611-136">runState</span></span>|[<span data-ttu-id="56611-137">runState</span><span class="sxs-lookup"><span data-stu-id="56611-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="56611-138">Estado da última execução do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="56611-138">State of latest run of the device management script.</span></span> <span data-ttu-id="56611-139">Os valores possíveis são: `unknown`, `success`, `fail`, `error`, `pending`.</span><span class="sxs-lookup"><span data-stu-id="56611-139">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="56611-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="56611-140">resultMessage</span></span>|<span data-ttu-id="56611-141">String</span><span class="sxs-lookup"><span data-stu-id="56611-141">String</span></span>|<span data-ttu-id="56611-142">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="56611-142">Details of execution output.</span></span>|
|<span data-ttu-id="56611-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="56611-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="56611-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56611-144">DateTimeOffset</span></span>|<span data-ttu-id="56611-145">Última vez em que o script de gerenciamento de dispositivos é executado.</span><span class="sxs-lookup"><span data-stu-id="56611-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="56611-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="56611-146">errorCode</span></span>|<span data-ttu-id="56611-147">Int32</span><span class="sxs-lookup"><span data-stu-id="56611-147">Int32</span></span>|<span data-ttu-id="56611-148">Código de erro correspondente à execução errada do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="56611-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="56611-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="56611-149">errorDescription</span></span>|<span data-ttu-id="56611-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56611-150">String</span></span>|<span data-ttu-id="56611-151">Descrição do erro correspondente à execução errada do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56611-151">Error description corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="56611-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="56611-152">lastSyncDateTime</span></span>|<span data-ttu-id="56611-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56611-153">DateTimeOffset</span></span>|<span data-ttu-id="56611-154">A última vez em que a extensão de gerenciamento do Intune é sincronizada com o Intune.</span><span class="sxs-lookup"><span data-stu-id="56611-154">The latest time that Intune Managment Extension syncs to Intune.</span></span>|
|<span data-ttu-id="56611-155">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="56611-155">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="56611-156">String</span><span class="sxs-lookup"><span data-stu-id="56611-156">String</span></span>|<span data-ttu-id="56611-157">Saída do script de detecção antes da correção.</span><span class="sxs-lookup"><span data-stu-id="56611-157">Output of the detection script before remediation.</span></span>|
|<span data-ttu-id="56611-158">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="56611-158">remediationScriptError</span></span>|<span data-ttu-id="56611-159">String</span><span class="sxs-lookup"><span data-stu-id="56611-159">String</span></span>|<span data-ttu-id="56611-160">Erro de saída do script de correção.</span><span class="sxs-lookup"><span data-stu-id="56611-160">Error output of the remediation script.</span></span>|
|<span data-ttu-id="56611-161">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="56611-161">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="56611-162">String</span><span class="sxs-lookup"><span data-stu-id="56611-162">String</span></span>|<span data-ttu-id="56611-163">A saída do script de detecção após a correção.</span><span class="sxs-lookup"><span data-stu-id="56611-163">Detection script output after remediation.</span></span>|



## <a name="response"></a><span data-ttu-id="56611-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="56611-164">Response</span></span>
<span data-ttu-id="56611-165">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56611-165">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56611-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56611-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="56611-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56611-167">Request</span></span>
<span data-ttu-id="56611-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56611-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="56611-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="56611-169">Response</span></span>
<span data-ttu-id="56611-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56611-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




