---
title: Atualizar deviceManagementIntentDeviceState
description: Atualiza as propriedades de um objeto deviceManagementIntentDeviceState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4711d0942ea1d0bb3dd6a328b747373bcf3e52c9
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522598"
---
# <a name="update-devicemanagementintentdevicestate"></a><span data-ttu-id="1aed2-103">Atualizar deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="1aed2-103">Update deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="1aed2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1aed2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aed2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1aed2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aed2-106">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1aed2-106">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1aed2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1aed2-107">Prerequisites</span></span>
<span data-ttu-id="1aed2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aed2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1aed2-110">Permission type</span></span>|<span data-ttu-id="1aed2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1aed2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aed2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1aed2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1aed2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aed2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1aed2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1aed2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aed2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aed2-115">Not supported.</span></span>|
|<span data-ttu-id="1aed2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aed2-116">Application</span></span>|<span data-ttu-id="1aed2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aed2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aed2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1aed2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="1aed2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1aed2-119">Request headers</span></span>
|<span data-ttu-id="1aed2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1aed2-120">Header</span></span>|<span data-ttu-id="1aed2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1aed2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aed2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1aed2-122">Authorization</span></span>|<span data-ttu-id="1aed2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1aed2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aed2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1aed2-124">Accept</span></span>|<span data-ttu-id="1aed2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1aed2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aed2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1aed2-126">Request body</span></span>
<span data-ttu-id="1aed2-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1aed2-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

<span data-ttu-id="1aed2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="1aed2-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>

|<span data-ttu-id="1aed2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aed2-129">Property</span></span>|<span data-ttu-id="1aed2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aed2-130">Type</span></span>|<span data-ttu-id="1aed2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aed2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aed2-132">id</span><span class="sxs-lookup"><span data-stu-id="1aed2-132">id</span></span>|<span data-ttu-id="1aed2-133">String</span><span class="sxs-lookup"><span data-stu-id="1aed2-133">String</span></span>|<span data-ttu-id="1aed2-134">A ID</span><span class="sxs-lookup"><span data-stu-id="1aed2-134">The ID</span></span>|
|<span data-ttu-id="1aed2-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1aed2-135">userPrincipalName</span></span>|<span data-ttu-id="1aed2-136">String</span><span class="sxs-lookup"><span data-stu-id="1aed2-136">String</span></span>|<span data-ttu-id="1aed2-137">O nome principal do usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="1aed2-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="1aed2-138">userName</span><span class="sxs-lookup"><span data-stu-id="1aed2-138">userName</span></span>|<span data-ttu-id="1aed2-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1aed2-139">String</span></span>|<span data-ttu-id="1aed2-140">O nome de usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="1aed2-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="1aed2-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1aed2-141">deviceDisplayName</span></span>|<span data-ttu-id="1aed2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1aed2-142">String</span></span>|<span data-ttu-id="1aed2-143">Nome do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="1aed2-143">Device name that is being reported</span></span>|
|<span data-ttu-id="1aed2-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1aed2-144">lastReportedDateTime</span></span>|<span data-ttu-id="1aed2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aed2-145">DateTimeOffset</span></span>|<span data-ttu-id="1aed2-146">Data e hora da última modificação de um relatório de intenção</span><span class="sxs-lookup"><span data-stu-id="1aed2-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="1aed2-147">state</span><span class="sxs-lookup"><span data-stu-id="1aed2-147">state</span></span>|[<span data-ttu-id="1aed2-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1aed2-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1aed2-149">Estado do dispositivo para uma intenção.</span><span class="sxs-lookup"><span data-stu-id="1aed2-149">Device state for an intent.</span></span> <span data-ttu-id="1aed2-150">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1aed2-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1aed2-151">deviceId</span><span class="sxs-lookup"><span data-stu-id="1aed2-151">deviceId</span></span>|<span data-ttu-id="1aed2-152">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1aed2-152">String</span></span>|<span data-ttu-id="1aed2-153">ID do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="1aed2-153">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="1aed2-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aed2-154">Response</span></span>
<span data-ttu-id="1aed2-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1aed2-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aed2-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1aed2-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aed2-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1aed2-157">Request</span></span>
<span data-ttu-id="1aed2-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1aed2-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="1aed2-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aed2-159">Response</span></span>
<span data-ttu-id="1aed2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1aed2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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







