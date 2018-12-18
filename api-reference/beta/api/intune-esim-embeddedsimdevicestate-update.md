---
title: Atualizar embeddedSIMDeviceState
description: Atualize as propriedades de um objeto embeddedSIMDeviceState.
author: tfitzmac
ms.openlocfilehash: 7c377199caae31bb45d65f0ad557cb27fb3916b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318519"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="2fac2-103">Atualizar embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="2fac2-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="2fac2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2fac2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fac2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2fac2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fac2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2fac2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fac2-107">Atualize as propriedades de um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="2fac2-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2fac2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2fac2-108">Prerequisites</span></span>
<span data-ttu-id="2fac2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fac2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fac2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fac2-111">Permission type</span></span>|<span data-ttu-id="2fac2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2fac2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fac2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fac2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fac2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fac2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fac2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fac2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fac2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fac2-116">Not supported.</span></span>|
|<span data-ttu-id="2fac2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fac2-117">Application</span></span>|<span data-ttu-id="2fac2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fac2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fac2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fac2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2fac2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fac2-120">Request headers</span></span>
|<span data-ttu-id="2fac2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fac2-121">Header</span></span>|<span data-ttu-id="2fac2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2fac2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fac2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fac2-123">Authorization</span></span>|<span data-ttu-id="2fac2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fac2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fac2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2fac2-125">Accept</span></span>|<span data-ttu-id="2fac2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fac2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fac2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fac2-127">Request body</span></span>
<span data-ttu-id="2fac2-128">No corpo da solicitação, fornece uma representação JSON para o objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="2fac2-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="2fac2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="2fac2-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="2fac2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fac2-130">Property</span></span>|<span data-ttu-id="2fac2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fac2-131">Type</span></span>|<span data-ttu-id="2fac2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fac2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fac2-133">id</span><span class="sxs-lookup"><span data-stu-id="2fac2-133">id</span></span>|<span data-ttu-id="2fac2-134">String</span><span class="sxs-lookup"><span data-stu-id="2fac2-134">String</span></span>|<span data-ttu-id="2fac2-135">Identificador exclusivo para o status do dispositivo SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="2fac2-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="2fac2-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="2fac2-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="2fac2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fac2-137">createdDateTime</span></span>|<span data-ttu-id="2fac2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fac2-138">DateTimeOffset</span></span>|<span data-ttu-id="2fac2-139">A hora em que o status do dispositivo SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="2fac2-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="2fac2-140">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="2fac2-140">Generated service side.</span></span>|
|<span data-ttu-id="2fac2-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fac2-141">modifiedDateTime</span></span>|<span data-ttu-id="2fac2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fac2-142">DateTimeOffset</span></span>|<span data-ttu-id="2fac2-143">A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2fac2-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="2fac2-144">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="2fac2-144">Updated service side.</span></span>|
|<span data-ttu-id="2fac2-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2fac2-145">lastSyncDateTime</span></span>|<span data-ttu-id="2fac2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fac2-146">DateTimeOffset</span></span>|<span data-ttu-id="2fac2-147">A hora em que o dispositivo SIM incorporado último check-in.</span><span class="sxs-lookup"><span data-stu-id="2fac2-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="2fac2-148">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="2fac2-148">Updated service side.</span></span>|
|<span data-ttu-id="2fac2-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="2fac2-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="2fac2-150">String</span><span class="sxs-lookup"><span data-stu-id="2fac2-150">String</span></span>|<span data-ttu-id="2fac2-151">O Universal circuito integrado cartão identificador (UICCID) que identifica o hardware no qual um perfil é a serem implantados.</span><span class="sxs-lookup"><span data-stu-id="2fac2-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="2fac2-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="2fac2-152">deviceName</span></span>|<span data-ttu-id="2fac2-153">String</span><span class="sxs-lookup"><span data-stu-id="2fac2-153">String</span></span>|<span data-ttu-id="2fac2-154">Nome do dispositivo para o qual a assinatura foi provisionado por exemplo, JOE de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="2fac2-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="2fac2-155">userName</span><span class="sxs-lookup"><span data-stu-id="2fac2-155">userName</span></span>|<span data-ttu-id="2fac2-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fac2-156">String</span></span>|<span data-ttu-id="2fac2-157">Nome de usuário que a assinatura foi provisionada para ex.: joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="2fac2-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="2fac2-158">estado</span><span class="sxs-lookup"><span data-stu-id="2fac2-158">state</span></span>|[<span data-ttu-id="2fac2-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="2fac2-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="2fac2-160">O estado da operação perfil aplicado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2fac2-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="2fac2-161">Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="2fac2-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="2fac2-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="2fac2-162">stateDetails</span></span>|<span data-ttu-id="2fac2-163">String</span><span class="sxs-lookup"><span data-stu-id="2fac2-163">String</span></span>|<span data-ttu-id="2fac2-164">Descrição do estado do provisionamento de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="2fac2-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="2fac2-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fac2-165">Response</span></span>
<span data-ttu-id="2fac2-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fac2-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fac2-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fac2-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fac2-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fac2-168">Request</span></span>
<span data-ttu-id="2fac2-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fac2-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 300

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="2fac2-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fac2-170">Response</span></span>
<span data-ttu-id="2fac2-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fac2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





