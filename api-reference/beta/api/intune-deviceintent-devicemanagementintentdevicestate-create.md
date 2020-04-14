---
title: Criar deviceManagementIntentDeviceState
description: Criar um novo objeto deviceManagementIntentDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f7e97cfe24e28fcc2cf8c423ab94fa14d707518
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326495"
---
# <a name="create-devicemanagementintentdevicestate"></a><span data-ttu-id="8d957-103">Criar deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="8d957-103">Create deviceManagementIntentDeviceState</span></span>

<span data-ttu-id="8d957-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d957-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d957-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d957-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d957-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d957-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d957-107">Criar um novo objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="8d957-107">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d957-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d957-108">Prerequisites</span></span>
<span data-ttu-id="8d957-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d957-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d957-111">Permission type</span></span>|<span data-ttu-id="8d957-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d957-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d957-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d957-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d957-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d957-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d957-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d957-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d957-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d957-116">Not supported.</span></span>|
|<span data-ttu-id="8d957-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d957-117">Application</span></span>|<span data-ttu-id="8d957-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d957-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d957-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d957-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="8d957-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d957-120">Request headers</span></span>
|<span data-ttu-id="8d957-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d957-121">Header</span></span>|<span data-ttu-id="8d957-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8d957-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d957-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d957-123">Authorization</span></span>|<span data-ttu-id="8d957-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d957-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d957-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d957-125">Accept</span></span>|<span data-ttu-id="8d957-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d957-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d957-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d957-127">Request body</span></span>
<span data-ttu-id="8d957-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntentDeviceState.</span><span class="sxs-lookup"><span data-stu-id="8d957-128">In the request body, supply a JSON representation for the deviceManagementIntentDeviceState object.</span></span>

<span data-ttu-id="8d957-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntentDeviceState.</span><span class="sxs-lookup"><span data-stu-id="8d957-129">The following table shows the properties that are required when you create the deviceManagementIntentDeviceState.</span></span>

|<span data-ttu-id="8d957-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d957-130">Property</span></span>|<span data-ttu-id="8d957-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d957-131">Type</span></span>|<span data-ttu-id="8d957-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d957-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d957-133">id</span><span class="sxs-lookup"><span data-stu-id="8d957-133">id</span></span>|<span data-ttu-id="8d957-134">String</span><span class="sxs-lookup"><span data-stu-id="8d957-134">String</span></span>|<span data-ttu-id="8d957-135">A ID</span><span class="sxs-lookup"><span data-stu-id="8d957-135">The ID</span></span>|
|<span data-ttu-id="8d957-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d957-136">userPrincipalName</span></span>|<span data-ttu-id="8d957-137">String</span><span class="sxs-lookup"><span data-stu-id="8d957-137">String</span></span>|<span data-ttu-id="8d957-138">O nome principal do usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="8d957-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="8d957-139">userName</span><span class="sxs-lookup"><span data-stu-id="8d957-139">userName</span></span>|<span data-ttu-id="8d957-140">String</span><span class="sxs-lookup"><span data-stu-id="8d957-140">String</span></span>|<span data-ttu-id="8d957-141">O nome de usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="8d957-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="8d957-142">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8d957-142">deviceDisplayName</span></span>|<span data-ttu-id="8d957-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d957-143">String</span></span>|<span data-ttu-id="8d957-144">Nome do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="8d957-144">Device name that is being reported</span></span>|
|<span data-ttu-id="8d957-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d957-145">lastReportedDateTime</span></span>|<span data-ttu-id="8d957-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d957-146">DateTimeOffset</span></span>|<span data-ttu-id="8d957-147">Data e hora da última modificação de um relatório de intenção</span><span class="sxs-lookup"><span data-stu-id="8d957-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="8d957-148">state</span><span class="sxs-lookup"><span data-stu-id="8d957-148">state</span></span>|[<span data-ttu-id="8d957-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8d957-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8d957-150">Estado do dispositivo para uma intenção.</span><span class="sxs-lookup"><span data-stu-id="8d957-150">Device state for an intent.</span></span> <span data-ttu-id="8d957-151">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8d957-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8d957-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="8d957-152">deviceId</span></span>|<span data-ttu-id="8d957-153">String</span><span class="sxs-lookup"><span data-stu-id="8d957-153">String</span></span>|<span data-ttu-id="8d957-154">ID do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="8d957-154">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="8d957-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d957-155">Response</span></span>
<span data-ttu-id="8d957-156">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d957-156">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d957-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d957-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d957-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d957-158">Request</span></span>
<span data-ttu-id="8d957-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d957-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="8d957-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d957-160">Response</span></span>
<span data-ttu-id="8d957-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d957-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "8db75881-5881-8db7-8158-b78d8158b78d",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```



