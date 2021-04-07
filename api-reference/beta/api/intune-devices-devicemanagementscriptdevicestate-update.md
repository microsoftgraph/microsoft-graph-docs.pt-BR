---
title: Atualizar deviceManagementScriptDeviceState
description: Atualize as propriedades de um objeto deviceManagementScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9014ae76127e37965b7f57d90bb39f4bdfa354fa
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611843"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="26398-103">Atualizar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26398-103">Update deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="26398-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26398-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26398-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26398-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26398-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26398-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26398-107">Atualize as propriedades de [um objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="26398-107">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26398-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26398-108">Prerequisites</span></span>
<span data-ttu-id="26398-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26398-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26398-111">Permission type</span></span>|<span data-ttu-id="26398-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26398-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26398-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26398-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26398-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26398-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="26398-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26398-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26398-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26398-116">Not supported.</span></span>|
|<span data-ttu-id="26398-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26398-117">Application</span></span>|<span data-ttu-id="26398-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26398-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26398-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26398-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="26398-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26398-120">Request headers</span></span>
|<span data-ttu-id="26398-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26398-121">Header</span></span>|<span data-ttu-id="26398-122">Valor</span><span class="sxs-lookup"><span data-stu-id="26398-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26398-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26398-123">Authorization</span></span>|<span data-ttu-id="26398-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26398-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26398-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26398-125">Accept</span></span>|<span data-ttu-id="26398-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26398-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26398-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26398-127">Request body</span></span>
<span data-ttu-id="26398-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="26398-128">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="26398-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="26398-129">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="26398-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26398-130">Property</span></span>|<span data-ttu-id="26398-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26398-131">Type</span></span>|<span data-ttu-id="26398-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26398-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26398-133">id</span><span class="sxs-lookup"><span data-stu-id="26398-133">id</span></span>|<span data-ttu-id="26398-134">String</span><span class="sxs-lookup"><span data-stu-id="26398-134">String</span></span>|<span data-ttu-id="26398-135">Chave da entidade de estado do dispositivo de script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26398-135">Key of the device management script device state entity.</span></span> <span data-ttu-id="26398-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26398-136">This property is read-only.</span></span>|
|<span data-ttu-id="26398-137">runState</span><span class="sxs-lookup"><span data-stu-id="26398-137">runState</span></span>|[<span data-ttu-id="26398-138">runState</span><span class="sxs-lookup"><span data-stu-id="26398-138">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="26398-139">Estado da última versão do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="26398-139">State of latest run of the device management script.</span></span> <span data-ttu-id="26398-140">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="26398-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="26398-141">resultMessage</span><span class="sxs-lookup"><span data-stu-id="26398-141">resultMessage</span></span>|<span data-ttu-id="26398-142">String</span><span class="sxs-lookup"><span data-stu-id="26398-142">String</span></span>|<span data-ttu-id="26398-143">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="26398-143">Details of execution output.</span></span>|
|<span data-ttu-id="26398-144">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="26398-144">lastStateUpdateDateTime</span></span>|<span data-ttu-id="26398-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26398-145">DateTimeOffset</span></span>|<span data-ttu-id="26398-146">Última hora em que o script de gerenciamento de dispositivos é executado.</span><span class="sxs-lookup"><span data-stu-id="26398-146">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="26398-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="26398-147">errorCode</span></span>|<span data-ttu-id="26398-148">Int32</span><span class="sxs-lookup"><span data-stu-id="26398-148">Int32</span></span>|<span data-ttu-id="26398-149">Código de erro correspondente à execução errônea do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26398-149">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="26398-150">errorDescription</span><span class="sxs-lookup"><span data-stu-id="26398-150">errorDescription</span></span>|<span data-ttu-id="26398-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26398-151">String</span></span>|<span data-ttu-id="26398-152">Descrição de erro correspondente à execução errônea do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26398-152">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="26398-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="26398-153">Response</span></span>
<span data-ttu-id="26398-154">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26398-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26398-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26398-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="26398-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26398-156">Request</span></span>
<span data-ttu-id="26398-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26398-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="26398-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="26398-158">Response</span></span>
<span data-ttu-id="26398-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26398-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




