---
title: Atualizar deviceComplianceScriptDeviceState
description: Atualize as propriedades de um objeto deviceComplianceScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d4f61c14eda8d1187acaab07d92975e07710ba5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130774"
---
# <a name="update-devicecompliancescriptdevicestate"></a><span data-ttu-id="5bb72-103">Atualizar deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="5bb72-103">Update deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="5bb72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bb72-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5bb72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bb72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5bb72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb72-107">Atualize as propriedades de [um objeto deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="5bb72-107">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bb72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5bb72-108">Prerequisites</span></span>
<span data-ttu-id="5bb72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bb72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bb72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bb72-111">Permission type</span></span>|<span data-ttu-id="5bb72-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bb72-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bb72-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bb72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5bb72-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb72-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5bb72-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bb72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bb72-116">Not supported.</span></span>|
|<span data-ttu-id="5bb72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bb72-117">Application</span></span>|<span data-ttu-id="5bb72-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb72-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bb72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bb72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5bb72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb72-120">Request headers</span></span>
|<span data-ttu-id="5bb72-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bb72-121">Header</span></span>|<span data-ttu-id="5bb72-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5bb72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bb72-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bb72-123">Authorization</span></span>|<span data-ttu-id="5bb72-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bb72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bb72-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5bb72-125">Accept</span></span>|<span data-ttu-id="5bb72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb72-127">Request body</span></span>
<span data-ttu-id="5bb72-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="5bb72-128">In the request body, supply a JSON representation for the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

<span data-ttu-id="5bb72-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="5bb72-129">The following table shows the properties that are required when you create the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>

|<span data-ttu-id="5bb72-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bb72-130">Property</span></span>|<span data-ttu-id="5bb72-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bb72-131">Type</span></span>|<span data-ttu-id="5bb72-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb72-133">id</span><span class="sxs-lookup"><span data-stu-id="5bb72-133">id</span></span>|<span data-ttu-id="5bb72-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb72-134">String</span></span>|<span data-ttu-id="5bb72-135">Chave da entidade de estado do dispositivo de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5bb72-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="5bb72-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5bb72-136">This property is read-only.</span></span>|
|<span data-ttu-id="5bb72-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="5bb72-137">detectionState</span></span>|[<span data-ttu-id="5bb72-138">runState</span><span class="sxs-lookup"><span data-stu-id="5bb72-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5bb72-139">Estado de detecção da última execução de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5bb72-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="5bb72-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="5bb72-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="5bb72-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb72-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="5bb72-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb72-142">DateTimeOffset</span></span>|<span data-ttu-id="5bb72-143">O último horário de quando o script de conformidade do dispositivo foi executado</span><span class="sxs-lookup"><span data-stu-id="5bb72-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="5bb72-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb72-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="5bb72-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb72-145">DateTimeOffset</span></span>|<span data-ttu-id="5bb72-146">O próximo horário de quando o script de conformidade do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="5bb72-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="5bb72-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb72-147">lastSyncDateTime</span></span>|<span data-ttu-id="5bb72-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb72-148">DateTimeOffset</span></span>|<span data-ttu-id="5bb72-149">A última vez que a Extensão de Managment do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="5bb72-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="5bb72-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="5bb72-150">scriptOutput</span></span>|<span data-ttu-id="5bb72-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb72-151">String</span></span>|<span data-ttu-id="5bb72-152">Saída do script de detecção</span><span class="sxs-lookup"><span data-stu-id="5bb72-152">Output of the detection script</span></span>|
|<span data-ttu-id="5bb72-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="5bb72-153">scriptError</span></span>|<span data-ttu-id="5bb72-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb72-154">String</span></span>|<span data-ttu-id="5bb72-155">Erro do script de detecção</span><span class="sxs-lookup"><span data-stu-id="5bb72-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="5bb72-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb72-156">Response</span></span>
<span data-ttu-id="5bb72-157">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bb72-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bb72-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bb72-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bb72-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb72-159">Request</span></span>
<span data-ttu-id="5bb72-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bb72-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="5bb72-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb72-161">Response</span></span>
<span data-ttu-id="5bb72-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bb72-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




