---
title: Criar deviceManagementScriptDeviceState
description: Criar um novo objeto deviceManagementScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343134224e37434d3c9be7e2fb32b5d2fcb1aae0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212947"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="a865b-103">Criar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a865b-103">Create deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="a865b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a865b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a865b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a865b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a865b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a865b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a865b-107">Criar um novo objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a865b-107">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a865b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a865b-108">Prerequisites</span></span>
<span data-ttu-id="a865b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a865b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a865b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a865b-111">Permission type</span></span>|<span data-ttu-id="a865b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a865b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a865b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a865b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a865b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a865b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a865b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a865b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a865b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a865b-116">Not supported.</span></span>|
|<span data-ttu-id="a865b-117">Application</span><span class="sxs-lookup"><span data-stu-id="a865b-117">Application</span></span>|<span data-ttu-id="a865b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a865b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a865b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a865b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="a865b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a865b-120">Request headers</span></span>
|<span data-ttu-id="a865b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a865b-121">Header</span></span>|<span data-ttu-id="a865b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a865b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a865b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a865b-123">Authorization</span></span>|<span data-ttu-id="a865b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a865b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a865b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a865b-125">Accept</span></span>|<span data-ttu-id="a865b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a865b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a865b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a865b-127">Request body</span></span>
<span data-ttu-id="a865b-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="a865b-128">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="a865b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="a865b-129">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="a865b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a865b-130">Property</span></span>|<span data-ttu-id="a865b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a865b-131">Type</span></span>|<span data-ttu-id="a865b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a865b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a865b-133">id</span><span class="sxs-lookup"><span data-stu-id="a865b-133">id</span></span>|<span data-ttu-id="a865b-134">String</span><span class="sxs-lookup"><span data-stu-id="a865b-134">String</span></span>|<span data-ttu-id="a865b-135">Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a865b-135">Key of the device management script device state entity.</span></span> <span data-ttu-id="a865b-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a865b-136">This property is read-only.</span></span>|
|<span data-ttu-id="a865b-137">runState</span><span class="sxs-lookup"><span data-stu-id="a865b-137">runState</span></span>|[<span data-ttu-id="a865b-138">runState</span><span class="sxs-lookup"><span data-stu-id="a865b-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="a865b-139">Estado da última execução do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a865b-139">State of latest run of the device management script.</span></span> <span data-ttu-id="a865b-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a865b-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="a865b-141">resultMessage</span><span class="sxs-lookup"><span data-stu-id="a865b-141">resultMessage</span></span>|<span data-ttu-id="a865b-142">String</span><span class="sxs-lookup"><span data-stu-id="a865b-142">String</span></span>|<span data-ttu-id="a865b-143">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="a865b-143">Details of execution output.</span></span>|
|<span data-ttu-id="a865b-144">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a865b-144">lastStateUpdateDateTime</span></span>|<span data-ttu-id="a865b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a865b-145">DateTimeOffset</span></span>|<span data-ttu-id="a865b-146">Última vez em que o script de gerenciamento de dispositivos é executado.</span><span class="sxs-lookup"><span data-stu-id="a865b-146">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="a865b-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="a865b-147">errorCode</span></span>|<span data-ttu-id="a865b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a865b-148">Int32</span></span>|<span data-ttu-id="a865b-149">Código de erro correspondente à execução errada do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a865b-149">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="a865b-150">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a865b-150">errorDescription</span></span>|<span data-ttu-id="a865b-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a865b-151">String</span></span>|<span data-ttu-id="a865b-152">Descrição do erro correspondente à execução errada do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a865b-152">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="a865b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a865b-153">Response</span></span>
<span data-ttu-id="a865b-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a865b-154">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a865b-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a865b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="a865b-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a865b-156">Request</span></span>
<span data-ttu-id="a865b-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a865b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="a865b-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="a865b-158">Response</span></span>
<span data-ttu-id="a865b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a865b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




