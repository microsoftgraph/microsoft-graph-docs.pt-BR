---
title: Criar embeddedSIMDeviceState
description: Crie um novo objeto EMBEDDEDSIMDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0627c0c011c193168b53c0efbe0274d7b0d2e91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126070"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="9e601-103">Criar embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9e601-103">Create embeddedSIMDeviceState</span></span>

<span data-ttu-id="9e601-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e601-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e601-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e601-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e601-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e601-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e601-107">Crie um novo [objeto EMBEDDEDSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="9e601-107">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e601-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e601-108">Prerequisites</span></span>
<span data-ttu-id="9e601-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e601-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e601-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e601-111">Permission type</span></span>|<span data-ttu-id="9e601-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e601-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e601-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e601-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e601-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e601-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e601-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e601-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e601-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e601-116">Not supported.</span></span>|
|<span data-ttu-id="9e601-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e601-117">Application</span></span>|<span data-ttu-id="9e601-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e601-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e601-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e601-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="9e601-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e601-120">Request headers</span></span>
|<span data-ttu-id="9e601-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e601-121">Header</span></span>|<span data-ttu-id="9e601-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9e601-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e601-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e601-123">Authorization</span></span>|<span data-ttu-id="9e601-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e601-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e601-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e601-125">Accept</span></span>|<span data-ttu-id="9e601-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e601-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e601-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e601-127">Request body</span></span>
<span data-ttu-id="9e601-128">No corpo da solicitação, fornece uma representação JSON para o objeto EMBEDDEDSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="9e601-128">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="9e601-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o embeddedSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="9e601-129">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="9e601-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e601-130">Property</span></span>|<span data-ttu-id="9e601-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e601-131">Type</span></span>|<span data-ttu-id="9e601-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e601-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e601-133">id</span><span class="sxs-lookup"><span data-stu-id="9e601-133">id</span></span>|<span data-ttu-id="9e601-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e601-134">String</span></span>|<span data-ttu-id="9e601-135">Identificador exclusivo para o status do dispositivo SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="9e601-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="9e601-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="9e601-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="9e601-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e601-137">createdDateTime</span></span>|<span data-ttu-id="9e601-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e601-138">DateTimeOffset</span></span>|<span data-ttu-id="9e601-139">A hora em que o status do dispositivo SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="9e601-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="9e601-140">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="9e601-140">Generated service side.</span></span>|
|<span data-ttu-id="9e601-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e601-141">modifiedDateTime</span></span>|<span data-ttu-id="9e601-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e601-142">DateTimeOffset</span></span>|<span data-ttu-id="9e601-143">A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9e601-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="9e601-144">Lado do serviço atualizado.</span><span class="sxs-lookup"><span data-stu-id="9e601-144">Updated service side.</span></span>|
|<span data-ttu-id="9e601-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9e601-145">lastSyncDateTime</span></span>|<span data-ttu-id="9e601-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e601-146">DateTimeOffset</span></span>|<span data-ttu-id="9e601-147">A última vez que o dispositivo SIM incorporado se registrou.</span><span class="sxs-lookup"><span data-stu-id="9e601-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="9e601-148">Lado do serviço atualizado.</span><span class="sxs-lookup"><span data-stu-id="9e601-148">Updated service side.</span></span>|
|<span data-ttu-id="9e601-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e601-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="9e601-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e601-150">String</span></span>|<span data-ttu-id="9e601-151">O Identificador de Placa de Circuito Integrado Universal (UICCID) identificando o hardware no qual um perfil deve ser implantado.</span><span class="sxs-lookup"><span data-stu-id="9e601-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="9e601-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="9e601-152">deviceName</span></span>|<span data-ttu-id="9e601-153">String</span><span class="sxs-lookup"><span data-stu-id="9e601-153">String</span></span>|<span data-ttu-id="9e601-154">Nome do dispositivo para o qual a assinatura foi provisionada, por exemplo, DESKTOP-JOE</span><span class="sxs-lookup"><span data-stu-id="9e601-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="9e601-155">userName</span><span class="sxs-lookup"><span data-stu-id="9e601-155">userName</span></span>|<span data-ttu-id="9e601-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e601-156">String</span></span>|<span data-ttu-id="9e601-157">Nome de usuário para o qual a assinatura foi provisionada, por exemplo, joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="9e601-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="9e601-158">state</span><span class="sxs-lookup"><span data-stu-id="9e601-158">state</span></span>|[<span data-ttu-id="9e601-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="9e601-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="9e601-160">O estado da operação de perfil aplicada ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e601-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="9e601-161">Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="9e601-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="9e601-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="9e601-162">stateDetails</span></span>|<span data-ttu-id="9e601-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e601-163">String</span></span>|<span data-ttu-id="9e601-164">Descrição da cadeia de caracteres do estado de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9e601-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="9e601-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e601-165">Response</span></span>
<span data-ttu-id="9e601-166">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto INCORPORADOSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e601-166">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e601-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e601-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e601-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e601-168">Request</span></span>
<span data-ttu-id="9e601-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e601-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e601-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e601-170">Response</span></span>
<span data-ttu-id="9e601-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e601-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




