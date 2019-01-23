---
title: Atualizar deviceManagementScriptDeviceState
description: Atualize as propriedades de um objeto deviceManagementScriptDeviceState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35768793279cdb96494a26dac8854f74e3c267ad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395150"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="bac93-103">Atualizar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="bac93-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="bac93-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bac93-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bac93-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bac93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bac93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bac93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac93-107">Atualize as propriedades de um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="bac93-107">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bac93-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bac93-108">Prerequisites</span></span>
<span data-ttu-id="bac93-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bac93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bac93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bac93-111">Permission type</span></span>|<span data-ttu-id="bac93-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bac93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bac93-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bac93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bac93-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bac93-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bac93-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bac93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bac93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bac93-116">Not supported.</span></span>|
|<span data-ttu-id="bac93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bac93-117">Application</span></span>|<span data-ttu-id="bac93-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bac93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bac93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bac93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="bac93-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bac93-120">Request headers</span></span>
|<span data-ttu-id="bac93-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bac93-121">Header</span></span>|<span data-ttu-id="bac93-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bac93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bac93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bac93-123">Authorization</span></span>|<span data-ttu-id="bac93-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bac93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bac93-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bac93-125">Accept</span></span>|<span data-ttu-id="bac93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bac93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bac93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bac93-127">Request body</span></span>
<span data-ttu-id="bac93-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="bac93-128">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="bac93-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="bac93-129">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="bac93-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bac93-130">Property</span></span>|<span data-ttu-id="bac93-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bac93-131">Type</span></span>|<span data-ttu-id="bac93-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bac93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac93-133">id</span><span class="sxs-lookup"><span data-stu-id="bac93-133">id</span></span>|<span data-ttu-id="bac93-134">String</span><span class="sxs-lookup"><span data-stu-id="bac93-134">String</span></span>|<span data-ttu-id="bac93-135">Chave da entidade de estado de dispositivo de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bac93-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="bac93-136">runState</span><span class="sxs-lookup"><span data-stu-id="bac93-136">runState</span></span>|[<span data-ttu-id="bac93-137">runState</span><span class="sxs-lookup"><span data-stu-id="bac93-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="bac93-138">Estado de execução mais recente do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bac93-138">State of latest run of the device management script.</span></span> <span data-ttu-id="bac93-139">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="bac93-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="bac93-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="bac93-140">resultMessage</span></span>|<span data-ttu-id="bac93-141">String</span><span class="sxs-lookup"><span data-stu-id="bac93-141">String</span></span>|<span data-ttu-id="bac93-142">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="bac93-142">Details of execution output.</span></span>|
|<span data-ttu-id="bac93-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bac93-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="bac93-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac93-144">DateTimeOffset</span></span>|<span data-ttu-id="bac93-145">Última vez em que o script de gerenciamento de dispositivo executa.</span><span class="sxs-lookup"><span data-stu-id="bac93-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="bac93-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="bac93-146">errorCode</span></span>|<span data-ttu-id="bac93-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bac93-147">Int32</span></span>|<span data-ttu-id="bac93-148">Código de erro correspondente à execução incorreta do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bac93-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="bac93-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="bac93-149">errorDescription</span></span>|<span data-ttu-id="bac93-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bac93-150">String</span></span>|<span data-ttu-id="bac93-151">Descrição do erro correspondente à execução incorreta do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bac93-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="bac93-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bac93-152">Response</span></span>
<span data-ttu-id="bac93-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bac93-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bac93-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bac93-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="bac93-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bac93-155">Request</span></span>
<span data-ttu-id="bac93-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bac93-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bac93-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="bac93-157">Response</span></span>
<span data-ttu-id="bac93-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bac93-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




