---
title: Atualizar deviceComplianceScriptDeviceState
description: Atualiza as propriedades de um objeto deviceComplianceScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2506199946b3b80c983c84486cb3b6de4a209494
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792440"
---
# <a name="update-devicecompliancescriptdevicestate"></a><span data-ttu-id="1d55e-103">Atualizar deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="1d55e-103">Update deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="1d55e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d55e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d55e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d55e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d55e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d55e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d55e-107">Atualiza as propriedades de um objeto [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1d55e-107">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d55e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d55e-108">Prerequisites</span></span>
<span data-ttu-id="1d55e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1d55e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1d55e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d55e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d55e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d55e-111">Permission type</span></span>|<span data-ttu-id="1d55e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d55e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d55e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d55e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d55e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d55e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1d55e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d55e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d55e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d55e-116">Not supported.</span></span>|
|<span data-ttu-id="1d55e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d55e-117">Application</span></span>|<span data-ttu-id="1d55e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d55e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d55e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d55e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="1d55e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d55e-120">Request headers</span></span>
|<span data-ttu-id="1d55e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d55e-121">Header</span></span>|<span data-ttu-id="1d55e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1d55e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d55e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d55e-123">Authorization</span></span>|<span data-ttu-id="1d55e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d55e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d55e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d55e-125">Accept</span></span>|<span data-ttu-id="1d55e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d55e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d55e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d55e-127">Request body</span></span>
<span data-ttu-id="1d55e-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1d55e-128">In the request body, supply a JSON representation for the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

<span data-ttu-id="1d55e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="1d55e-129">The following table shows the properties that are required when you create the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>

|<span data-ttu-id="1d55e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d55e-130">Property</span></span>|<span data-ttu-id="1d55e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d55e-131">Type</span></span>|<span data-ttu-id="1d55e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d55e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d55e-133">id</span><span class="sxs-lookup"><span data-stu-id="1d55e-133">id</span></span>|<span data-ttu-id="1d55e-134">String</span><span class="sxs-lookup"><span data-stu-id="1d55e-134">String</span></span>|<span data-ttu-id="1d55e-135">Chave da entidade de estado do dispositivo de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d55e-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="1d55e-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d55e-136">This property is read-only.</span></span>|
|<span data-ttu-id="1d55e-137">detecçaostate</span><span class="sxs-lookup"><span data-stu-id="1d55e-137">detectionState</span></span>|[<span data-ttu-id="1d55e-138">runState</span><span class="sxs-lookup"><span data-stu-id="1d55e-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="1d55e-139">Estado de detecção da execução do script de conformidade do dispositivo mais recente.</span><span class="sxs-lookup"><span data-stu-id="1d55e-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="1d55e-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="1d55e-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="1d55e-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1d55e-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="1d55e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d55e-142">DateTimeOffset</span></span>|<span data-ttu-id="1d55e-143">O último carimbo de data/hora de quando o script de conformidade do dispositivo foi executado</span><span class="sxs-lookup"><span data-stu-id="1d55e-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="1d55e-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1d55e-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="1d55e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d55e-145">DateTimeOffset</span></span>|<span data-ttu-id="1d55e-146">O carimbo de data/hora seguinte de quando o script de conformidade do dispositivo deve ser executado</span><span class="sxs-lookup"><span data-stu-id="1d55e-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="1d55e-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1d55e-147">lastSyncDateTime</span></span>|<span data-ttu-id="1d55e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d55e-148">DateTimeOffset</span></span>|<span data-ttu-id="1d55e-149">A última vez em que a extensão de gerenciamento do Intune foi sincronizada com o Intune</span><span class="sxs-lookup"><span data-stu-id="1d55e-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="1d55e-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="1d55e-150">scriptOutput</span></span>|<span data-ttu-id="1d55e-151">String</span><span class="sxs-lookup"><span data-stu-id="1d55e-151">String</span></span>|<span data-ttu-id="1d55e-152">Saída do script de detecção</span><span class="sxs-lookup"><span data-stu-id="1d55e-152">Output of the detection script</span></span>|
|<span data-ttu-id="1d55e-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="1d55e-153">scriptError</span></span>|<span data-ttu-id="1d55e-154">String</span><span class="sxs-lookup"><span data-stu-id="1d55e-154">String</span></span>|<span data-ttu-id="1d55e-155">Erro do script de detecção</span><span class="sxs-lookup"><span data-stu-id="1d55e-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="1d55e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d55e-156">Response</span></span>
<span data-ttu-id="1d55e-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d55e-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d55e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d55e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d55e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d55e-159">Request</span></span>
<span data-ttu-id="1d55e-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d55e-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d55e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d55e-161">Response</span></span>
<span data-ttu-id="1d55e-162">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1d55e-162">Here is an example of the response.</span></span> <span data-ttu-id="1d55e-163">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1d55e-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1d55e-164">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1d55e-164">All of the properties will be returned from an actual call.</span></span>
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



