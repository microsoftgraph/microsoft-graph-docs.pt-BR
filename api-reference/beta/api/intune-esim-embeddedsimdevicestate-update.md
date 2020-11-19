---
title: Atualizar embeddedSIMDeviceState
description: Atualiza as propriedades de um objeto embeddedSIMDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 446f3430b5ea2fa6904522951c3831a21bc01b92
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233711"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="598a5-103">Atualizar embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="598a5-103">Update embeddedSIMDeviceState</span></span>

<span data-ttu-id="598a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="598a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="598a5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="598a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="598a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="598a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="598a5-107">Atualiza as propriedades de um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="598a5-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="598a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="598a5-108">Prerequisites</span></span>
<span data-ttu-id="598a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="598a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="598a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="598a5-111">Permission type</span></span>|<span data-ttu-id="598a5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="598a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="598a5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="598a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="598a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="598a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="598a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="598a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="598a5-116">Not supported.</span></span>|
|<span data-ttu-id="598a5-117">Application</span><span class="sxs-lookup"><span data-stu-id="598a5-117">Application</span></span>|<span data-ttu-id="598a5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598a5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="598a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="598a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="598a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="598a5-120">Request headers</span></span>
|<span data-ttu-id="598a5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="598a5-121">Header</span></span>|<span data-ttu-id="598a5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="598a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="598a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="598a5-123">Authorization</span></span>|<span data-ttu-id="598a5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="598a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="598a5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="598a5-125">Accept</span></span>|<span data-ttu-id="598a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="598a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="598a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="598a5-127">Request body</span></span>
<span data-ttu-id="598a5-128">No corpo da solicitação, forneça uma representação JSON do objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="598a5-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="598a5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="598a5-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="598a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="598a5-130">Property</span></span>|<span data-ttu-id="598a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="598a5-131">Type</span></span>|<span data-ttu-id="598a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="598a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="598a5-133">id</span><span class="sxs-lookup"><span data-stu-id="598a5-133">id</span></span>|<span data-ttu-id="598a5-134">String</span><span class="sxs-lookup"><span data-stu-id="598a5-134">String</span></span>|<span data-ttu-id="598a5-135">Identificador exclusivo para o status do dispositivo SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="598a5-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="598a5-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="598a5-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="598a5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="598a5-137">createdDateTime</span></span>|<span data-ttu-id="598a5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598a5-138">DateTimeOffset</span></span>|<span data-ttu-id="598a5-139">A hora em que o status do dispositivo SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="598a5-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="598a5-140">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="598a5-140">Generated service side.</span></span>|
|<span data-ttu-id="598a5-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="598a5-141">modifiedDateTime</span></span>|<span data-ttu-id="598a5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598a5-142">DateTimeOffset</span></span>|<span data-ttu-id="598a5-143">A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="598a5-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="598a5-144">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="598a5-144">Updated service side.</span></span>|
|<span data-ttu-id="598a5-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="598a5-145">lastSyncDateTime</span></span>|<span data-ttu-id="598a5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598a5-146">DateTimeOffset</span></span>|<span data-ttu-id="598a5-147">A hora em que o dispositivo SIM incorporado foi verificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="598a5-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="598a5-148">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="598a5-148">Updated service side.</span></span>|
|<span data-ttu-id="598a5-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="598a5-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="598a5-150">String</span><span class="sxs-lookup"><span data-stu-id="598a5-150">String</span></span>|<span data-ttu-id="598a5-151">O identificador de cartão de circuito integrado universal (UICCID) identificando o hardware no qual um perfil deve ser implantado.</span><span class="sxs-lookup"><span data-stu-id="598a5-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="598a5-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="598a5-152">deviceName</span></span>|<span data-ttu-id="598a5-153">String</span><span class="sxs-lookup"><span data-stu-id="598a5-153">String</span></span>|<span data-ttu-id="598a5-154">Nome do dispositivo para o qual a assinatura foi provisionada, por exemplo, DESKTOP-JOE</span><span class="sxs-lookup"><span data-stu-id="598a5-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="598a5-155">userName</span><span class="sxs-lookup"><span data-stu-id="598a5-155">userName</span></span>|<span data-ttu-id="598a5-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="598a5-156">String</span></span>|<span data-ttu-id="598a5-157">Nome de usuário para o qual a assinatura foi provisionada, por exemplo, joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="598a5-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="598a5-158">state</span><span class="sxs-lookup"><span data-stu-id="598a5-158">state</span></span>|[<span data-ttu-id="598a5-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="598a5-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="598a5-160">O estado da operação de perfil aplicada ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="598a5-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="598a5-161">Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="598a5-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="598a5-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="598a5-162">stateDetails</span></span>|<span data-ttu-id="598a5-163">String</span><span class="sxs-lookup"><span data-stu-id="598a5-163">String</span></span>|<span data-ttu-id="598a5-164">Descrição da cadeia de caracteres do estado de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="598a5-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="598a5-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="598a5-165">Response</span></span>
<span data-ttu-id="598a5-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="598a5-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="598a5-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="598a5-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="598a5-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="598a5-168">Request</span></span>
<span data-ttu-id="598a5-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="598a5-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="598a5-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="598a5-170">Response</span></span>
<span data-ttu-id="598a5-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="598a5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




