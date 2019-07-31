---
title: Atualizar deviceManagementScriptDeviceState
description: Atualiza as propriedades de um objeto deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db46807d376decdcbe81484ce097514af849efa7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986012"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="92a4b-103">Atualizar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="92a4b-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="92a4b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92a4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92a4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92a4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92a4b-106">Atualiza as propriedades de um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="92a4b-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92a4b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92a4b-107">Prerequisites</span></span>
<span data-ttu-id="92a4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92a4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92a4b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92a4b-110">Permission type</span></span>|<span data-ttu-id="92a4b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92a4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92a4b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92a4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92a4b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92a4b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="92a4b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92a4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92a4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92a4b-115">Not supported.</span></span>|
|<span data-ttu-id="92a4b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92a4b-116">Application</span></span>|<span data-ttu-id="92a4b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92a4b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92a4b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92a4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="92a4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92a4b-119">Request headers</span></span>
|<span data-ttu-id="92a4b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92a4b-120">Header</span></span>|<span data-ttu-id="92a4b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="92a4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92a4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="92a4b-122">Authorization</span></span>|<span data-ttu-id="92a4b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92a4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92a4b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92a4b-124">Accept</span></span>|<span data-ttu-id="92a4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92a4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92a4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92a4b-126">Request body</span></span>
<span data-ttu-id="92a4b-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="92a4b-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="92a4b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="92a4b-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="92a4b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92a4b-129">Property</span></span>|<span data-ttu-id="92a4b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="92a4b-130">Type</span></span>|<span data-ttu-id="92a4b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="92a4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a4b-132">id</span><span class="sxs-lookup"><span data-stu-id="92a4b-132">id</span></span>|<span data-ttu-id="92a4b-133">String</span><span class="sxs-lookup"><span data-stu-id="92a4b-133">String</span></span>|<span data-ttu-id="92a4b-134">Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="92a4b-134">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="92a4b-135">runState</span><span class="sxs-lookup"><span data-stu-id="92a4b-135">runState</span></span>|[<span data-ttu-id="92a4b-136">runState</span><span class="sxs-lookup"><span data-stu-id="92a4b-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="92a4b-137">Estado da última execução do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="92a4b-137">State of latest run of the device management script.</span></span> <span data-ttu-id="92a4b-138">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="92a4b-138">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="92a4b-139">resultMessage</span><span class="sxs-lookup"><span data-stu-id="92a4b-139">resultMessage</span></span>|<span data-ttu-id="92a4b-140">String</span><span class="sxs-lookup"><span data-stu-id="92a4b-140">String</span></span>|<span data-ttu-id="92a4b-141">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="92a4b-141">Details of execution output.</span></span>|
|<span data-ttu-id="92a4b-142">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="92a4b-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="92a4b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92a4b-143">DateTimeOffset</span></span>|<span data-ttu-id="92a4b-144">Última vez em que o script de gerenciamento de dispositivos é executado.</span><span class="sxs-lookup"><span data-stu-id="92a4b-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="92a4b-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="92a4b-145">errorCode</span></span>|<span data-ttu-id="92a4b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="92a4b-146">Int32</span></span>|<span data-ttu-id="92a4b-147">Código de erro correspondente à execução errada do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="92a4b-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="92a4b-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="92a4b-148">errorDescription</span></span>|<span data-ttu-id="92a4b-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92a4b-149">String</span></span>|<span data-ttu-id="92a4b-150">Descrição do erro correspondente à execução errada do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92a4b-150">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="92a4b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a4b-151">Response</span></span>
<span data-ttu-id="92a4b-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92a4b-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92a4b-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92a4b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="92a4b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92a4b-154">Request</span></span>
<span data-ttu-id="92a4b-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92a4b-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="92a4b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a4b-156">Response</span></span>
<span data-ttu-id="92a4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92a4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





