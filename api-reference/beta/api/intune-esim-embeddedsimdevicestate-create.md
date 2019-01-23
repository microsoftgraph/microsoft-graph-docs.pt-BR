---
title: Criar embeddedSIMDeviceState
description: Crie um novo objeto de embeddedSIMDeviceState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 451f40d7ad23787311e4a0b9ed3c046cbe34b830
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413413"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="d10e5-103">Criar embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="d10e5-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="d10e5-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d10e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d10e5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d10e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d10e5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d10e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d10e5-107">Crie um novo objeto de [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d10e5-107">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d10e5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d10e5-108">Prerequisites</span></span>
<span data-ttu-id="d10e5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d10e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d10e5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d10e5-111">Permission type</span></span>|<span data-ttu-id="d10e5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d10e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d10e5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d10e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d10e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d10e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d10e5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d10e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d10e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d10e5-116">Not supported.</span></span>|
|<span data-ttu-id="d10e5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d10e5-117">Application</span></span>|<span data-ttu-id="d10e5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d10e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d10e5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d10e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="d10e5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d10e5-120">Request headers</span></span>
|<span data-ttu-id="d10e5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d10e5-121">Header</span></span>|<span data-ttu-id="d10e5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d10e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d10e5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d10e5-123">Authorization</span></span>|<span data-ttu-id="d10e5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d10e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d10e5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d10e5-125">Accept</span></span>|<span data-ttu-id="d10e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d10e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d10e5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d10e5-127">Request body</span></span>
<span data-ttu-id="d10e5-128">No corpo da solicitação, fornece uma representação JSON para o objeto embeddedSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="d10e5-128">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="d10e5-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o embeddedSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="d10e5-129">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="d10e5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d10e5-130">Property</span></span>|<span data-ttu-id="d10e5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d10e5-131">Type</span></span>|<span data-ttu-id="d10e5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d10e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d10e5-133">id</span><span class="sxs-lookup"><span data-stu-id="d10e5-133">id</span></span>|<span data-ttu-id="d10e5-134">String</span><span class="sxs-lookup"><span data-stu-id="d10e5-134">String</span></span>|<span data-ttu-id="d10e5-135">Identificador exclusivo para o status do dispositivo SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="d10e5-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="d10e5-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="d10e5-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d10e5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d10e5-137">createdDateTime</span></span>|<span data-ttu-id="d10e5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10e5-138">DateTimeOffset</span></span>|<span data-ttu-id="d10e5-139">A hora em que o status do dispositivo SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="d10e5-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="d10e5-140">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="d10e5-140">Generated service side.</span></span>|
|<span data-ttu-id="d10e5-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d10e5-141">modifiedDateTime</span></span>|<span data-ttu-id="d10e5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10e5-142">DateTimeOffset</span></span>|<span data-ttu-id="d10e5-143">A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d10e5-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="d10e5-144">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="d10e5-144">Updated service side.</span></span>|
|<span data-ttu-id="d10e5-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d10e5-145">lastSyncDateTime</span></span>|<span data-ttu-id="d10e5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10e5-146">DateTimeOffset</span></span>|<span data-ttu-id="d10e5-147">A hora em que o dispositivo SIM incorporado último check-in.</span><span class="sxs-lookup"><span data-stu-id="d10e5-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="d10e5-148">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="d10e5-148">Updated service side.</span></span>|
|<span data-ttu-id="d10e5-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="d10e5-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="d10e5-150">String</span><span class="sxs-lookup"><span data-stu-id="d10e5-150">String</span></span>|<span data-ttu-id="d10e5-151">O Universal circuito integrado cartão identificador (UICCID) que identifica o hardware no qual um perfil é a serem implantados.</span><span class="sxs-lookup"><span data-stu-id="d10e5-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="d10e5-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="d10e5-152">deviceName</span></span>|<span data-ttu-id="d10e5-153">String</span><span class="sxs-lookup"><span data-stu-id="d10e5-153">String</span></span>|<span data-ttu-id="d10e5-154">Nome do dispositivo para o qual a assinatura foi provisionado por exemplo, JOE de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="d10e5-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="d10e5-155">userName</span><span class="sxs-lookup"><span data-stu-id="d10e5-155">userName</span></span>|<span data-ttu-id="d10e5-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d10e5-156">String</span></span>|<span data-ttu-id="d10e5-157">Nome de usuário que a assinatura foi provisionada para ex.: joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="d10e5-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="d10e5-158">estado</span><span class="sxs-lookup"><span data-stu-id="d10e5-158">state</span></span>|[<span data-ttu-id="d10e5-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="d10e5-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="d10e5-160">O estado da operação perfil aplicado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d10e5-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="d10e5-161">Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="d10e5-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="d10e5-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="d10e5-162">stateDetails</span></span>|<span data-ttu-id="d10e5-163">String</span><span class="sxs-lookup"><span data-stu-id="d10e5-163">String</span></span>|<span data-ttu-id="d10e5-164">Descrição do estado do provisionamento de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d10e5-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="d10e5-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d10e5-165">Response</span></span>
<span data-ttu-id="d10e5-166">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d10e5-166">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d10e5-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d10e5-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="d10e5-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d10e5-168">Request</span></span>
<span data-ttu-id="d10e5-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d10e5-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d10e5-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="d10e5-170">Response</span></span>
<span data-ttu-id="d10e5-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d10e5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




