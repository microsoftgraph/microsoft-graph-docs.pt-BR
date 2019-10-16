---
title: Criar deviceManagementScriptDeviceState
description: Criar um novo objeto deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfd0b21906cd7692e32b93475efdb8b861ed44b3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530612"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="1031d-103">Criar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="1031d-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="1031d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1031d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1031d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1031d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1031d-106">Criar um novo objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1031d-106">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1031d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1031d-107">Prerequisites</span></span>
<span data-ttu-id="1031d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1031d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1031d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1031d-110">Permission type</span></span>|<span data-ttu-id="1031d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1031d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1031d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1031d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1031d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1031d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1031d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1031d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1031d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1031d-115">Not supported.</span></span>|
|<span data-ttu-id="1031d-116">Application</span><span class="sxs-lookup"><span data-stu-id="1031d-116">Application</span></span>|<span data-ttu-id="1031d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1031d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1031d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1031d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="1031d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1031d-119">Request headers</span></span>
|<span data-ttu-id="1031d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1031d-120">Header</span></span>|<span data-ttu-id="1031d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1031d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1031d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1031d-122">Authorization</span></span>|<span data-ttu-id="1031d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1031d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1031d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1031d-124">Accept</span></span>|<span data-ttu-id="1031d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1031d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1031d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1031d-126">Request body</span></span>
<span data-ttu-id="1031d-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="1031d-127">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="1031d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="1031d-128">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="1031d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1031d-129">Property</span></span>|<span data-ttu-id="1031d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1031d-130">Type</span></span>|<span data-ttu-id="1031d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1031d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1031d-132">id</span><span class="sxs-lookup"><span data-stu-id="1031d-132">id</span></span>|<span data-ttu-id="1031d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1031d-133">String</span></span>|<span data-ttu-id="1031d-134">Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1031d-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="1031d-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1031d-135">This property is read-only.</span></span>|
|<span data-ttu-id="1031d-136">runState</span><span class="sxs-lookup"><span data-stu-id="1031d-136">runState</span></span>|[<span data-ttu-id="1031d-137">runState</span><span class="sxs-lookup"><span data-stu-id="1031d-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="1031d-138">Estado da última execução do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1031d-138">State of latest run of the device management script.</span></span> <span data-ttu-id="1031d-139">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="1031d-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="1031d-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="1031d-140">resultMessage</span></span>|<span data-ttu-id="1031d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1031d-141">String</span></span>|<span data-ttu-id="1031d-142">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="1031d-142">Details of execution output.</span></span>|
|<span data-ttu-id="1031d-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1031d-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="1031d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1031d-144">DateTimeOffset</span></span>|<span data-ttu-id="1031d-145">Última vez em que o script de gerenciamento de dispositivos é executado.</span><span class="sxs-lookup"><span data-stu-id="1031d-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="1031d-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="1031d-146">errorCode</span></span>|<span data-ttu-id="1031d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1031d-147">Int32</span></span>|<span data-ttu-id="1031d-148">Código de erro correspondente à execução errada do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1031d-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="1031d-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="1031d-149">errorDescription</span></span>|<span data-ttu-id="1031d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1031d-150">String</span></span>|<span data-ttu-id="1031d-151">Descrição do erro correspondente à execução errada do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1031d-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="1031d-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="1031d-152">Response</span></span>
<span data-ttu-id="1031d-153">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1031d-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1031d-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1031d-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="1031d-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1031d-155">Request</span></span>
<span data-ttu-id="1031d-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1031d-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

### <a name="response"></a><span data-ttu-id="1031d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1031d-157">Response</span></span>
<span data-ttu-id="1031d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1031d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```






