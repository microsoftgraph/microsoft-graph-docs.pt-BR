---
title: Criar deviceManagementScriptDeviceState
description: Crie um novo objeto de deviceManagementScriptDeviceState.
author: tfitzmac
ms.openlocfilehash: 2b809c82e077bc75c354d3b8b1c09548eaacad64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304847"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="777cc-103">Criar deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="777cc-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="777cc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="777cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="777cc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="777cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="777cc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="777cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="777cc-107">Crie um novo objeto de [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="777cc-107">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="777cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="777cc-108">Prerequisites</span></span>
<span data-ttu-id="777cc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="777cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="777cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="777cc-111">Permission type</span></span>|<span data-ttu-id="777cc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="777cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="777cc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="777cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="777cc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="777cc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="777cc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="777cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="777cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="777cc-116">Not supported.</span></span>|
|<span data-ttu-id="777cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="777cc-117">Application</span></span>|<span data-ttu-id="777cc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="777cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="777cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="777cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="777cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="777cc-120">Request headers</span></span>
|<span data-ttu-id="777cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="777cc-121">Header</span></span>|<span data-ttu-id="777cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="777cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="777cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="777cc-123">Authorization</span></span>|<span data-ttu-id="777cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="777cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="777cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="777cc-125">Accept</span></span>|<span data-ttu-id="777cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="777cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="777cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="777cc-127">Request body</span></span>
<span data-ttu-id="777cc-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="777cc-128">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="777cc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="777cc-129">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="777cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="777cc-130">Property</span></span>|<span data-ttu-id="777cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="777cc-131">Type</span></span>|<span data-ttu-id="777cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="777cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="777cc-133">id</span><span class="sxs-lookup"><span data-stu-id="777cc-133">id</span></span>|<span data-ttu-id="777cc-134">String</span><span class="sxs-lookup"><span data-stu-id="777cc-134">String</span></span>|<span data-ttu-id="777cc-135">Chave da entidade de estado de dispositivo de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="777cc-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="777cc-136">runState</span><span class="sxs-lookup"><span data-stu-id="777cc-136">runState</span></span>|[<span data-ttu-id="777cc-137">runState</span><span class="sxs-lookup"><span data-stu-id="777cc-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="777cc-138">Estado de execução mais recente do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="777cc-138">State of latest run of the device management script.</span></span> <span data-ttu-id="777cc-139">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="777cc-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="777cc-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="777cc-140">resultMessage</span></span>|<span data-ttu-id="777cc-141">String</span><span class="sxs-lookup"><span data-stu-id="777cc-141">String</span></span>|<span data-ttu-id="777cc-142">Detalhes da saída de execução.</span><span class="sxs-lookup"><span data-stu-id="777cc-142">Details of execution output.</span></span>|
|<span data-ttu-id="777cc-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="777cc-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="777cc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="777cc-144">DateTimeOffset</span></span>|<span data-ttu-id="777cc-145">Última vez em que o script de gerenciamento de dispositivo executa.</span><span class="sxs-lookup"><span data-stu-id="777cc-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="777cc-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="777cc-146">errorCode</span></span>|<span data-ttu-id="777cc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="777cc-147">Int32</span></span>|<span data-ttu-id="777cc-148">Código de erro correspondente à execução incorreta do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="777cc-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="777cc-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="777cc-149">errorDescription</span></span>|<span data-ttu-id="777cc-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777cc-150">String</span></span>|<span data-ttu-id="777cc-151">Descrição do erro correspondente à execução incorreta do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="777cc-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="777cc-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="777cc-152">Response</span></span>
<span data-ttu-id="777cc-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="777cc-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="777cc-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="777cc-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="777cc-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="777cc-155">Request</span></span>
<span data-ttu-id="777cc-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="777cc-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="777cc-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="777cc-157">Response</span></span>
<span data-ttu-id="777cc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="777cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





