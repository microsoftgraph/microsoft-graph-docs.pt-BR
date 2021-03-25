---
title: Atualizar userExperienceAnalyticsNotAutopilotReadyDevice
description: Atualize as propriedades de um objeto userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f65af4455834540609854708078bd8b62cbb6a1d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159350"
---
# <a name="update-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="6a9cc-103">Atualizar userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="6a9cc-103">Update userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="6a9cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a9cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a9cc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a9cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a9cc-107">Atualize as propriedades de [um objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-107">Update the properties of a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a9cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a9cc-108">Prerequisites</span></span>
<span data-ttu-id="6a9cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a9cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a9cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a9cc-111">Permission type</span></span>|<span data-ttu-id="6a9cc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a9cc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a9cc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9cc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6a9cc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a9cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-116">Not supported.</span></span>|
|<span data-ttu-id="6a9cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a9cc-117">Application</span></span>|<span data-ttu-id="6a9cc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9cc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a9cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a9cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="6a9cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9cc-120">Request headers</span></span>
|<span data-ttu-id="6a9cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a9cc-121">Header</span></span>|<span data-ttu-id="6a9cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a9cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a9cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a9cc-123">Authorization</span></span>|<span data-ttu-id="6a9cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a9cc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a9cc-125">Accept</span></span>|<span data-ttu-id="6a9cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a9cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a9cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9cc-127">Request body</span></span>
<span data-ttu-id="6a9cc-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

<span data-ttu-id="6a9cc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a9cc-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md).</span></span>

|<span data-ttu-id="6a9cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a9cc-130">Property</span></span>|<span data-ttu-id="6a9cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a9cc-131">Type</span></span>|<span data-ttu-id="6a9cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a9cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a9cc-133">id</span><span class="sxs-lookup"><span data-stu-id="6a9cc-133">id</span></span>|<span data-ttu-id="6a9cc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a9cc-134">String</span></span>|<span data-ttu-id="6a9cc-135">O identificador exclusivo do dispositivo intune de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-135">The unique identifier of the user experience analytics intune device.</span></span>|
|<span data-ttu-id="6a9cc-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="6a9cc-136">deviceName</span></span>|<span data-ttu-id="6a9cc-137">String</span><span class="sxs-lookup"><span data-stu-id="6a9cc-137">String</span></span>|<span data-ttu-id="6a9cc-138">O nome do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-138">The intune device's name.</span></span>|
|<span data-ttu-id="6a9cc-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6a9cc-139">serialNumber</span></span>|<span data-ttu-id="6a9cc-140">String</span><span class="sxs-lookup"><span data-stu-id="6a9cc-140">String</span></span>|<span data-ttu-id="6a9cc-141">O número de série do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-141">The intune device's serial number.</span></span>|
|<span data-ttu-id="6a9cc-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="6a9cc-142">manufacturer</span></span>|<span data-ttu-id="6a9cc-143">String</span><span class="sxs-lookup"><span data-stu-id="6a9cc-143">String</span></span>|<span data-ttu-id="6a9cc-144">O fabricante do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-144">The intune device's manufacturer.</span></span>|
|<span data-ttu-id="6a9cc-145">modelo</span><span class="sxs-lookup"><span data-stu-id="6a9cc-145">model</span></span>|<span data-ttu-id="6a9cc-146">String</span><span class="sxs-lookup"><span data-stu-id="6a9cc-146">String</span></span>|<span data-ttu-id="6a9cc-147">O modelo do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-147">The intune device's model.</span></span>|
|<span data-ttu-id="6a9cc-148">managedBy</span><span class="sxs-lookup"><span data-stu-id="6a9cc-148">managedBy</span></span>|<span data-ttu-id="6a9cc-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a9cc-149">String</span></span>|<span data-ttu-id="6a9cc-150">O dispositivo do intune é gerenciado por.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-150">The intune device's managed by.</span></span>|
|<span data-ttu-id="6a9cc-151">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="6a9cc-151">autoPilotRegistered</span></span>|<span data-ttu-id="6a9cc-152">Booleano</span><span class="sxs-lookup"><span data-stu-id="6a9cc-152">Boolean</span></span>|<span data-ttu-id="6a9cc-153">O piloto automático do dispositivo intuneRegistered.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-153">The intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="6a9cc-154">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="6a9cc-154">autoPilotProfileAssigned</span></span>|<span data-ttu-id="6a9cc-155">Booleano</span><span class="sxs-lookup"><span data-stu-id="6a9cc-155">Boolean</span></span>|<span data-ttu-id="6a9cc-156">O autopilotProfileAssigned do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-156">The intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="6a9cc-157">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="6a9cc-157">azureAdRegistered</span></span>|[<span data-ttu-id="6a9cc-158">azureAdRegisteredState</span><span class="sxs-lookup"><span data-stu-id="6a9cc-158">azureAdRegisteredState</span></span>](../resources/intune-devices-azureadregisteredstate.md)|<span data-ttu-id="6a9cc-159">O dispositivo do intune é azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-159">The intune device's azureAdRegistered.</span></span> <span data-ttu-id="6a9cc-160">Os valores possíveis são: `no`, `yes`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-160">Possible values are: `no`, `yes`, `unknown`.</span></span>|
|<span data-ttu-id="6a9cc-161">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="6a9cc-161">azureAdJoinType</span></span>|<span data-ttu-id="6a9cc-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a9cc-162">String</span></span>|<span data-ttu-id="6a9cc-163">O azure Ad joinType do dispositivo do intune.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-163">The intune device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="6a9cc-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9cc-164">Response</span></span>
<span data-ttu-id="6a9cc-165">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-165">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a9cc-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a9cc-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a9cc-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9cc-167">Request</span></span>
<span data-ttu-id="6a9cc-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": "yes",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="6a9cc-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9cc-169">Response</span></span>
<span data-ttu-id="6a9cc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "11c3ffd7-ffd7-11c3-d7ff-c311d7ffc311",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": "yes",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




