---
title: Atualizar deviceManagementIntentDeviceState
description: Atualiza as propriedades de um objeto deviceManagementIntentDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30b5963b806c8e3f11c4aa0737e4f4599866be39
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945729"
---
# <a name="update-devicemanagementintentdevicestate"></a><span data-ttu-id="d656f-103">Atualizar deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="d656f-103">Update deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="d656f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d656f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d656f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d656f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d656f-106">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d656f-106">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d656f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d656f-107">Prerequisites</span></span>
<span data-ttu-id="d656f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d656f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d656f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d656f-110">Permission type</span></span>|<span data-ttu-id="d656f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d656f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d656f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d656f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d656f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d656f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d656f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d656f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d656f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d656f-115">Not supported.</span></span>|
|<span data-ttu-id="d656f-116">Application</span><span class="sxs-lookup"><span data-stu-id="d656f-116">Application</span></span>|<span data-ttu-id="d656f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d656f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d656f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d656f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d656f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d656f-119">Request headers</span></span>
|<span data-ttu-id="d656f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d656f-120">Header</span></span>|<span data-ttu-id="d656f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d656f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d656f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d656f-122">Authorization</span></span>|<span data-ttu-id="d656f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d656f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d656f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d656f-124">Accept</span></span>|<span data-ttu-id="d656f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d656f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d656f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d656f-126">Request body</span></span>
<span data-ttu-id="d656f-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d656f-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

<span data-ttu-id="d656f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="d656f-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>

|<span data-ttu-id="d656f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d656f-129">Property</span></span>|<span data-ttu-id="d656f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d656f-130">Type</span></span>|<span data-ttu-id="d656f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d656f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d656f-132">id</span><span class="sxs-lookup"><span data-stu-id="d656f-132">id</span></span>|<span data-ttu-id="d656f-133">String</span><span class="sxs-lookup"><span data-stu-id="d656f-133">String</span></span>|<span data-ttu-id="d656f-134">A ID</span><span class="sxs-lookup"><span data-stu-id="d656f-134">The ID</span></span>|
|<span data-ttu-id="d656f-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d656f-135">userPrincipalName</span></span>|<span data-ttu-id="d656f-136">String</span><span class="sxs-lookup"><span data-stu-id="d656f-136">String</span></span>|<span data-ttu-id="d656f-137">O nome principal do usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="d656f-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="d656f-138">userName</span><span class="sxs-lookup"><span data-stu-id="d656f-138">userName</span></span>|<span data-ttu-id="d656f-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d656f-139">String</span></span>|<span data-ttu-id="d656f-140">O nome de usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="d656f-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="d656f-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d656f-141">deviceDisplayName</span></span>|<span data-ttu-id="d656f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d656f-142">String</span></span>|<span data-ttu-id="d656f-143">Nome do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d656f-143">Device name that is being reported</span></span>|
|<span data-ttu-id="d656f-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d656f-144">lastReportedDateTime</span></span>|<span data-ttu-id="d656f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d656f-145">DateTimeOffset</span></span>|<span data-ttu-id="d656f-146">Data e hora da última modificação de um relatório de intenção</span><span class="sxs-lookup"><span data-stu-id="d656f-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="d656f-147">state</span><span class="sxs-lookup"><span data-stu-id="d656f-147">state</span></span>|[<span data-ttu-id="d656f-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d656f-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d656f-149">Estado do dispositivo para uma intenção.</span><span class="sxs-lookup"><span data-stu-id="d656f-149">Device state for an intent.</span></span> <span data-ttu-id="d656f-150">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d656f-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d656f-151">deviceId</span><span class="sxs-lookup"><span data-stu-id="d656f-151">deviceId</span></span>|<span data-ttu-id="d656f-152">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d656f-152">String</span></span>|<span data-ttu-id="d656f-153">ID do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="d656f-153">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="d656f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d656f-154">Response</span></span>
<span data-ttu-id="d656f-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d656f-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d656f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d656f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d656f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d656f-157">Request</span></span>
<span data-ttu-id="d656f-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d656f-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d656f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d656f-159">Response</span></span>
<span data-ttu-id="d656f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d656f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





