---
title: Criar embeddedSIMDeviceState
description: Crie um novo objeto de embeddedSIMDeviceState.
ms.openlocfilehash: 3d52c8910d38f72e9c08e27fe694cea49796b884
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039648"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="41d1c-103">Criar embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="41d1c-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="41d1c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="41d1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41d1c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41d1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41d1c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41d1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41d1c-107">Crie um novo objeto de [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="41d1c-107">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41d1c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41d1c-108">Prerequisites</span></span>
<span data-ttu-id="41d1c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d1c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41d1c-111">Permission type</span></span>|<span data-ttu-id="41d1c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41d1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41d1c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41d1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41d1c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41d1c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41d1c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41d1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41d1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41d1c-116">Not supported.</span></span>|
|<span data-ttu-id="41d1c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41d1c-117">Application</span></span>|<span data-ttu-id="41d1c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41d1c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41d1c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41d1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="41d1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41d1c-120">Request headers</span></span>
|<span data-ttu-id="41d1c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41d1c-121">Header</span></span>|<span data-ttu-id="41d1c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="41d1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41d1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41d1c-123">Authorization</span></span>|<span data-ttu-id="41d1c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41d1c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41d1c-125">Accept</span></span>|<span data-ttu-id="41d1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41d1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41d1c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41d1c-127">Request body</span></span>
<span data-ttu-id="41d1c-128">No corpo da solicitação, fornece uma representação JSON para o objeto embeddedSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="41d1c-128">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="41d1c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o embeddedSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="41d1c-129">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="41d1c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41d1c-130">Property</span></span>|<span data-ttu-id="41d1c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="41d1c-131">Type</span></span>|<span data-ttu-id="41d1c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="41d1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d1c-133">id</span><span class="sxs-lookup"><span data-stu-id="41d1c-133">id</span></span>|<span data-ttu-id="41d1c-134">String</span><span class="sxs-lookup"><span data-stu-id="41d1c-134">String</span></span>|<span data-ttu-id="41d1c-135">Identificador exclusivo para o status do dispositivo SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="41d1c-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="41d1c-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="41d1c-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="41d1c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41d1c-137">createdDateTime</span></span>|<span data-ttu-id="41d1c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41d1c-138">DateTimeOffset</span></span>|<span data-ttu-id="41d1c-139">A hora em que o status do dispositivo SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="41d1c-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="41d1c-140">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="41d1c-140">Generated service side.</span></span>|
|<span data-ttu-id="41d1c-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41d1c-141">modifiedDateTime</span></span>|<span data-ttu-id="41d1c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41d1c-142">DateTimeOffset</span></span>|<span data-ttu-id="41d1c-143">A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="41d1c-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="41d1c-144">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="41d1c-144">Updated service side.</span></span>|
|<span data-ttu-id="41d1c-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="41d1c-145">lastSyncDateTime</span></span>|<span data-ttu-id="41d1c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41d1c-146">DateTimeOffset</span></span>|<span data-ttu-id="41d1c-147">A hora em que o dispositivo SIM incorporado último check-in.</span><span class="sxs-lookup"><span data-stu-id="41d1c-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="41d1c-148">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="41d1c-148">Updated service side.</span></span>|
|<span data-ttu-id="41d1c-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="41d1c-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="41d1c-150">String</span><span class="sxs-lookup"><span data-stu-id="41d1c-150">String</span></span>|<span data-ttu-id="41d1c-151">O Universal circuito integrado cartão identificador (UICCID) que identifica o hardware no qual um perfil é a serem implantados.</span><span class="sxs-lookup"><span data-stu-id="41d1c-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="41d1c-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="41d1c-152">deviceName</span></span>|<span data-ttu-id="41d1c-153">String</span><span class="sxs-lookup"><span data-stu-id="41d1c-153">String</span></span>|<span data-ttu-id="41d1c-154">Nome do dispositivo para o qual a assinatura foi provisionado por exemplo, JOE de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="41d1c-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="41d1c-155">userName</span><span class="sxs-lookup"><span data-stu-id="41d1c-155">userName</span></span>|<span data-ttu-id="41d1c-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41d1c-156">String</span></span>|<span data-ttu-id="41d1c-157">Nome de usuário que a assinatura foi provisionada para ex.: joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="41d1c-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="41d1c-158">state</span><span class="sxs-lookup"><span data-stu-id="41d1c-158">state</span></span>|[<span data-ttu-id="41d1c-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="41d1c-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="41d1c-160">O estado da operação perfil aplicado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41d1c-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="41d1c-161">Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="41d1c-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="41d1c-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="41d1c-162">stateDetails</span></span>|<span data-ttu-id="41d1c-163">String</span><span class="sxs-lookup"><span data-stu-id="41d1c-163">String</span></span>|<span data-ttu-id="41d1c-164">Descrição do estado do provisionamento de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="41d1c-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="41d1c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d1c-165">Response</span></span>
<span data-ttu-id="41d1c-166">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41d1c-166">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d1c-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41d1c-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="41d1c-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41d1c-168">Request</span></span>
<span data-ttu-id="41d1c-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41d1c-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="41d1c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d1c-170">Response</span></span>
<span data-ttu-id="41d1c-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41d1c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```





