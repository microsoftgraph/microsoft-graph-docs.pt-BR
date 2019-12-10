---
title: Atualizar embeddedSIMDeviceState
description: Atualiza as propriedades de um objeto embeddedSIMDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bf7a48ccef44f8bcb2c9cb8d7753afe339b17d8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943520"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="24212-103">Atualizar embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="24212-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="24212-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24212-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24212-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24212-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24212-106">Atualiza as propriedades de um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="24212-106">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24212-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24212-107">Prerequisites</span></span>
<span data-ttu-id="24212-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24212-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24212-110">Permission type</span></span>|<span data-ttu-id="24212-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24212-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24212-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24212-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24212-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24212-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24212-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24212-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24212-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24212-115">Not supported.</span></span>|
|<span data-ttu-id="24212-116">Application</span><span class="sxs-lookup"><span data-stu-id="24212-116">Application</span></span>|<span data-ttu-id="24212-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24212-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24212-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24212-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="24212-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24212-119">Request headers</span></span>
|<span data-ttu-id="24212-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24212-120">Header</span></span>|<span data-ttu-id="24212-121">Valor</span><span class="sxs-lookup"><span data-stu-id="24212-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24212-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24212-122">Authorization</span></span>|<span data-ttu-id="24212-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24212-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24212-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24212-124">Accept</span></span>|<span data-ttu-id="24212-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24212-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24212-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24212-126">Request body</span></span>
<span data-ttu-id="24212-127">No corpo da solicitação, forneça uma representação JSON do objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="24212-127">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="24212-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="24212-128">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="24212-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24212-129">Property</span></span>|<span data-ttu-id="24212-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="24212-130">Type</span></span>|<span data-ttu-id="24212-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="24212-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24212-132">id</span><span class="sxs-lookup"><span data-stu-id="24212-132">id</span></span>|<span data-ttu-id="24212-133">String</span><span class="sxs-lookup"><span data-stu-id="24212-133">String</span></span>|<span data-ttu-id="24212-134">Identificador exclusivo para o status do dispositivo SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="24212-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="24212-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="24212-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="24212-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24212-136">createdDateTime</span></span>|<span data-ttu-id="24212-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24212-137">DateTimeOffset</span></span>|<span data-ttu-id="24212-138">A hora em que o status do dispositivo SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="24212-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="24212-139">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="24212-139">Generated service side.</span></span>|
|<span data-ttu-id="24212-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24212-140">modifiedDateTime</span></span>|<span data-ttu-id="24212-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24212-141">DateTimeOffset</span></span>|<span data-ttu-id="24212-142">A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="24212-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="24212-143">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="24212-143">Updated service side.</span></span>|
|<span data-ttu-id="24212-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="24212-144">lastSyncDateTime</span></span>|<span data-ttu-id="24212-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24212-145">DateTimeOffset</span></span>|<span data-ttu-id="24212-146">A hora em que o dispositivo SIM incorporado foi verificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="24212-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="24212-147">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="24212-147">Updated service side.</span></span>|
|<span data-ttu-id="24212-148">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="24212-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="24212-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="24212-149">String</span></span>|<span data-ttu-id="24212-150">O identificador de cartão de circuito integrado universal (UICCID) identificando o hardware no qual um perfil deve ser implantado.</span><span class="sxs-lookup"><span data-stu-id="24212-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="24212-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="24212-151">deviceName</span></span>|<span data-ttu-id="24212-152">String</span><span class="sxs-lookup"><span data-stu-id="24212-152">String</span></span>|<span data-ttu-id="24212-153">Nome do dispositivo para o qual a assinatura foi provisionada, por exemplo, DESKTOP-JOE</span><span class="sxs-lookup"><span data-stu-id="24212-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="24212-154">userName</span><span class="sxs-lookup"><span data-stu-id="24212-154">userName</span></span>|<span data-ttu-id="24212-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24212-155">String</span></span>|<span data-ttu-id="24212-156">Nome de usuário para o qual a assinatura foi provisionada, por exemplo, joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="24212-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="24212-157">state</span><span class="sxs-lookup"><span data-stu-id="24212-157">state</span></span>|[<span data-ttu-id="24212-158">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="24212-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="24212-159">O estado da operação de perfil aplicada ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="24212-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="24212-160">Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="24212-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="24212-161">stateDetails</span><span class="sxs-lookup"><span data-stu-id="24212-161">stateDetails</span></span>|<span data-ttu-id="24212-162">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="24212-162">String</span></span>|<span data-ttu-id="24212-163">Descrição da cadeia de caracteres do estado de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="24212-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="24212-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="24212-164">Response</span></span>
<span data-ttu-id="24212-165">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24212-165">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24212-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24212-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="24212-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24212-167">Request</span></span>
<span data-ttu-id="24212-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24212-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="24212-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="24212-169">Response</span></span>
<span data-ttu-id="24212-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24212-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





