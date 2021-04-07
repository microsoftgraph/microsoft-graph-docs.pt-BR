---
title: Criar deviceComplianceScriptDeviceState
description: Crie um novo objeto deviceComplianceScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0dcb977cc83eedeab5c0a8f8ac1cb3ccc96d8f32
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611850"
---
# <a name="create-devicecompliancescriptdevicestate"></a><span data-ttu-id="2ab3e-103">Criar deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2ab3e-103">Create deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="2ab3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ab3e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ab3e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab3e-107">Crie um novo [objeto deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="2ab3e-107">Create a new [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ab3e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ab3e-108">Prerequisites</span></span>
<span data-ttu-id="2ab3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ab3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ab3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ab3e-111">Permission type</span></span>|<span data-ttu-id="2ab3e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ab3e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ab3e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ab3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ab3e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab3e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2ab3e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ab3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ab3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-116">Not supported.</span></span>|
|<span data-ttu-id="2ab3e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ab3e-117">Application</span></span>|<span data-ttu-id="2ab3e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab3e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ab3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ab3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="2ab3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ab3e-120">Request headers</span></span>
|<span data-ttu-id="2ab3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ab3e-121">Header</span></span>|<span data-ttu-id="2ab3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2ab3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ab3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ab3e-123">Authorization</span></span>|<span data-ttu-id="2ab3e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ab3e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ab3e-125">Accept</span></span>|<span data-ttu-id="2ab3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ab3e-127">Request body</span></span>
<span data-ttu-id="2ab3e-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceComplianceScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-128">In the request body, supply a JSON representation for the deviceComplianceScriptDeviceState object.</span></span>

<span data-ttu-id="2ab3e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-129">The following table shows the properties that are required when you create the deviceComplianceScriptDeviceState.</span></span>

|<span data-ttu-id="2ab3e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ab3e-130">Property</span></span>|<span data-ttu-id="2ab3e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ab3e-131">Type</span></span>|<span data-ttu-id="2ab3e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ab3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab3e-133">id</span><span class="sxs-lookup"><span data-stu-id="2ab3e-133">id</span></span>|<span data-ttu-id="2ab3e-134">String</span><span class="sxs-lookup"><span data-stu-id="2ab3e-134">String</span></span>|<span data-ttu-id="2ab3e-135">Chave da entidade de estado do dispositivo de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="2ab3e-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-136">This property is read-only.</span></span>|
|<span data-ttu-id="2ab3e-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="2ab3e-137">detectionState</span></span>|[<span data-ttu-id="2ab3e-138">runState</span><span class="sxs-lookup"><span data-stu-id="2ab3e-138">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="2ab3e-139">Estado de detecção da última execução de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="2ab3e-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="2ab3e-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab3e-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="2ab3e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab3e-142">DateTimeOffset</span></span>|<span data-ttu-id="2ab3e-143">O último horário de quando o script de conformidade do dispositivo foi executado</span><span class="sxs-lookup"><span data-stu-id="2ab3e-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="2ab3e-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab3e-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="2ab3e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab3e-145">DateTimeOffset</span></span>|<span data-ttu-id="2ab3e-146">O próximo horário de quando o script de conformidade do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="2ab3e-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="2ab3e-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab3e-147">lastSyncDateTime</span></span>|<span data-ttu-id="2ab3e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab3e-148">DateTimeOffset</span></span>|<span data-ttu-id="2ab3e-149">A última vez que a Extensão de Managment do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="2ab3e-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="2ab3e-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="2ab3e-150">scriptOutput</span></span>|<span data-ttu-id="2ab3e-151">String</span><span class="sxs-lookup"><span data-stu-id="2ab3e-151">String</span></span>|<span data-ttu-id="2ab3e-152">Saída do script de detecção</span><span class="sxs-lookup"><span data-stu-id="2ab3e-152">Output of the detection script</span></span>|
|<span data-ttu-id="2ab3e-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="2ab3e-153">scriptError</span></span>|<span data-ttu-id="2ab3e-154">String</span><span class="sxs-lookup"><span data-stu-id="2ab3e-154">String</span></span>|<span data-ttu-id="2ab3e-155">Erro do script de detecção</span><span class="sxs-lookup"><span data-stu-id="2ab3e-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="2ab3e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ab3e-156">Response</span></span>
<span data-ttu-id="2ab3e-157">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab3e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ab3e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ab3e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ab3e-159">Request</span></span>
<span data-ttu-id="2ab3e-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```

### <a name="response"></a><span data-ttu-id="2ab3e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ab3e-161">Response</span></span>
<span data-ttu-id="2ab3e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ab3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 436

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "7bd39c86-9c86-7bd3-869c-d37b869cd37b",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```




