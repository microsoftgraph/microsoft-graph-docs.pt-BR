---
title: Atualizar deviceManagementIntentDeviceState
description: Atualize as propriedades de um objeto deviceManagementIntentDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c89aaa9ab1e442079294820746bb1cc2f3a2d36b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150812"
---
# <a name="update-devicemanagementintentdevicestate"></a><span data-ttu-id="dd82b-103">Atualizar deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="dd82b-103">Update deviceManagementIntentDeviceState</span></span>

<span data-ttu-id="dd82b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd82b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd82b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd82b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd82b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd82b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd82b-107">Atualize as propriedades de [um objeto deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="dd82b-107">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd82b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd82b-108">Prerequisites</span></span>
<span data-ttu-id="dd82b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd82b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd82b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd82b-111">Permission type</span></span>|<span data-ttu-id="dd82b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd82b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd82b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd82b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd82b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd82b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd82b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd82b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd82b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd82b-116">Not supported.</span></span>|
|<span data-ttu-id="dd82b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd82b-117">Application</span></span>|<span data-ttu-id="dd82b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd82b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd82b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd82b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="dd82b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd82b-120">Request headers</span></span>
|<span data-ttu-id="dd82b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd82b-121">Header</span></span>|<span data-ttu-id="dd82b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dd82b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd82b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd82b-123">Authorization</span></span>|<span data-ttu-id="dd82b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd82b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd82b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd82b-125">Accept</span></span>|<span data-ttu-id="dd82b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd82b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd82b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd82b-127">Request body</span></span>
<span data-ttu-id="dd82b-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="dd82b-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

<span data-ttu-id="dd82b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="dd82b-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>

|<span data-ttu-id="dd82b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd82b-130">Property</span></span>|<span data-ttu-id="dd82b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd82b-131">Type</span></span>|<span data-ttu-id="dd82b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd82b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd82b-133">id</span><span class="sxs-lookup"><span data-stu-id="dd82b-133">id</span></span>|<span data-ttu-id="dd82b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd82b-134">String</span></span>|<span data-ttu-id="dd82b-135">A ID</span><span class="sxs-lookup"><span data-stu-id="dd82b-135">The ID</span></span>|
|<span data-ttu-id="dd82b-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd82b-136">userPrincipalName</span></span>|<span data-ttu-id="dd82b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd82b-137">String</span></span>|<span data-ttu-id="dd82b-138">O nome principal do usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="dd82b-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="dd82b-139">userName</span><span class="sxs-lookup"><span data-stu-id="dd82b-139">userName</span></span>|<span data-ttu-id="dd82b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd82b-140">String</span></span>|<span data-ttu-id="dd82b-141">O nome de usuário que está sendo relatado em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="dd82b-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="dd82b-142">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd82b-142">deviceDisplayName</span></span>|<span data-ttu-id="dd82b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd82b-143">String</span></span>|<span data-ttu-id="dd82b-144">Nome do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="dd82b-144">Device name that is being reported</span></span>|
|<span data-ttu-id="dd82b-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd82b-145">lastReportedDateTime</span></span>|<span data-ttu-id="dd82b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd82b-146">DateTimeOffset</span></span>|<span data-ttu-id="dd82b-147">Data da última modificação de um relatório de intenção</span><span class="sxs-lookup"><span data-stu-id="dd82b-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="dd82b-148">state</span><span class="sxs-lookup"><span data-stu-id="dd82b-148">state</span></span>|[<span data-ttu-id="dd82b-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dd82b-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dd82b-150">Estado do dispositivo para uma intenção.</span><span class="sxs-lookup"><span data-stu-id="dd82b-150">Device state for an intent.</span></span> <span data-ttu-id="dd82b-151">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dd82b-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dd82b-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="dd82b-152">deviceId</span></span>|<span data-ttu-id="dd82b-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd82b-153">String</span></span>|<span data-ttu-id="dd82b-154">ID do dispositivo que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="dd82b-154">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="dd82b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd82b-155">Response</span></span>
<span data-ttu-id="dd82b-156">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd82b-156">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd82b-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd82b-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd82b-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd82b-158">Request</span></span>
<span data-ttu-id="dd82b-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd82b-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dd82b-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd82b-160">Response</span></span>
<span data-ttu-id="dd82b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd82b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




