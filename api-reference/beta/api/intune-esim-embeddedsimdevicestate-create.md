---
title: Criar embeddedSIMDeviceState
description: Criar um novo objeto embeddedSIMDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48fa960c2ca22b52e161947b509cc8eaec355c11
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983481"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="460cc-103">Criar embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="460cc-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="460cc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="460cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="460cc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="460cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="460cc-106">Criar um novo objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="460cc-106">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="460cc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="460cc-107">Prerequisites</span></span>
<span data-ttu-id="460cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="460cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="460cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="460cc-110">Permission type</span></span>|<span data-ttu-id="460cc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="460cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="460cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="460cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="460cc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460cc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="460cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="460cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="460cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="460cc-115">Not supported.</span></span>|
|<span data-ttu-id="460cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="460cc-116">Application</span></span>|<span data-ttu-id="460cc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="460cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="460cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="460cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="460cc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="460cc-119">Request headers</span></span>
|<span data-ttu-id="460cc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="460cc-120">Header</span></span>|<span data-ttu-id="460cc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="460cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="460cc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="460cc-122">Authorization</span></span>|<span data-ttu-id="460cc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="460cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="460cc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="460cc-124">Accept</span></span>|<span data-ttu-id="460cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="460cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="460cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="460cc-126">Request body</span></span>
<span data-ttu-id="460cc-127">No corpo da solicitação, forneça uma representação JSON do objeto embeddedSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="460cc-127">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="460cc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar embeddedSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="460cc-128">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="460cc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="460cc-129">Property</span></span>|<span data-ttu-id="460cc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="460cc-130">Type</span></span>|<span data-ttu-id="460cc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="460cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="460cc-132">id</span><span class="sxs-lookup"><span data-stu-id="460cc-132">id</span></span>|<span data-ttu-id="460cc-133">String</span><span class="sxs-lookup"><span data-stu-id="460cc-133">String</span></span>|<span data-ttu-id="460cc-134">Identificador exclusivo para o status do dispositivo SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="460cc-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="460cc-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="460cc-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="460cc-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="460cc-136">createdDateTime</span></span>|<span data-ttu-id="460cc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="460cc-137">DateTimeOffset</span></span>|<span data-ttu-id="460cc-138">A hora em que o status do dispositivo SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="460cc-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="460cc-139">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="460cc-139">Generated service side.</span></span>|
|<span data-ttu-id="460cc-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="460cc-140">modifiedDateTime</span></span>|<span data-ttu-id="460cc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="460cc-141">DateTimeOffset</span></span>|<span data-ttu-id="460cc-142">A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="460cc-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="460cc-143">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="460cc-143">Updated service side.</span></span>|
|<span data-ttu-id="460cc-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="460cc-144">lastSyncDateTime</span></span>|<span data-ttu-id="460cc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="460cc-145">DateTimeOffset</span></span>|<span data-ttu-id="460cc-146">A hora em que o dispositivo SIM incorporado foi verificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="460cc-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="460cc-147">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="460cc-147">Updated service side.</span></span>|
|<span data-ttu-id="460cc-148">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="460cc-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="460cc-149">String</span><span class="sxs-lookup"><span data-stu-id="460cc-149">String</span></span>|<span data-ttu-id="460cc-150">O identificador de cartão de circuito integrado universal (UICCID) identificando o hardware no qual um perfil deve ser implantado.</span><span class="sxs-lookup"><span data-stu-id="460cc-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="460cc-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="460cc-151">deviceName</span></span>|<span data-ttu-id="460cc-152">String</span><span class="sxs-lookup"><span data-stu-id="460cc-152">String</span></span>|<span data-ttu-id="460cc-153">Nome do dispositivo para o qual a assinatura foi provisionada, por exemplo, DESKTOP-JOE</span><span class="sxs-lookup"><span data-stu-id="460cc-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="460cc-154">userName</span><span class="sxs-lookup"><span data-stu-id="460cc-154">userName</span></span>|<span data-ttu-id="460cc-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="460cc-155">String</span></span>|<span data-ttu-id="460cc-156">Nome de usuário para o qual a assinatura foi provisionada, por exemplo, joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="460cc-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="460cc-157">estado</span><span class="sxs-lookup"><span data-stu-id="460cc-157">state</span></span>|[<span data-ttu-id="460cc-158">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="460cc-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="460cc-159">O estado da operação de perfil aplicada ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="460cc-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="460cc-160">Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="460cc-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="460cc-161">stateDetails</span><span class="sxs-lookup"><span data-stu-id="460cc-161">stateDetails</span></span>|<span data-ttu-id="460cc-162">String</span><span class="sxs-lookup"><span data-stu-id="460cc-162">String</span></span>|<span data-ttu-id="460cc-163">Descrição da cadeia de caracteres do estado de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="460cc-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="460cc-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="460cc-164">Response</span></span>
<span data-ttu-id="460cc-165">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="460cc-165">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="460cc-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="460cc-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="460cc-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="460cc-167">Request</span></span>
<span data-ttu-id="460cc-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="460cc-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="460cc-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="460cc-169">Response</span></span>
<span data-ttu-id="460cc-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="460cc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





