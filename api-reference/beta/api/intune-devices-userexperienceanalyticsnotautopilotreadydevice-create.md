---
title: Criar userExperienceAnalyticsNotAutopilotReadyDevice
description: Crie um novo objeto userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3842a478ab89e03366a111a52aed901613959dce
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159338"
---
# <a name="create-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="2cfb4-103">Criar userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="2cfb4-103">Create userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="2cfb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cfb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cfb4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cfb4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cfb4-107">Crie um novo [objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="2cfb4-107">Create a new [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cfb4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2cfb4-108">Prerequisites</span></span>
<span data-ttu-id="2cfb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cfb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cfb4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cfb4-111">Permission type</span></span>|<span data-ttu-id="2cfb4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2cfb4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cfb4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cfb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cfb4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cfb4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2cfb4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cfb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cfb4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-116">Not supported.</span></span>|
|<span data-ttu-id="2cfb4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cfb4-117">Application</span></span>|<span data-ttu-id="2cfb4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cfb4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cfb4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cfb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a><span data-ttu-id="2cfb4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cfb4-120">Request headers</span></span>
|<span data-ttu-id="2cfb4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2cfb4-121">Header</span></span>|<span data-ttu-id="2cfb4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2cfb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cfb4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cfb4-123">Authorization</span></span>|<span data-ttu-id="2cfb4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cfb4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2cfb4-125">Accept</span></span>|<span data-ttu-id="2cfb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cfb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cfb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cfb4-127">Request body</span></span>
<span data-ttu-id="2cfb4-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-128">In the request body, supply a JSON representation for the userExperienceAnalyticsNotAutopilotReadyDevice object.</span></span>

<span data-ttu-id="2cfb4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-129">The following table shows the properties that are required when you create the userExperienceAnalyticsNotAutopilotReadyDevice.</span></span>

|<span data-ttu-id="2cfb4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cfb4-130">Property</span></span>|<span data-ttu-id="2cfb4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cfb4-131">Type</span></span>|<span data-ttu-id="2cfb4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cfb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cfb4-133">id</span><span class="sxs-lookup"><span data-stu-id="2cfb4-133">id</span></span>|<span data-ttu-id="2cfb4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cfb4-134">String</span></span>|<span data-ttu-id="2cfb4-135">O identificador exclusivo do dispositivo intune de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-135">The unique identifier of the user experience analytics intune device.</span></span>|
|<span data-ttu-id="2cfb4-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="2cfb4-136">deviceName</span></span>|<span data-ttu-id="2cfb4-137">String</span><span class="sxs-lookup"><span data-stu-id="2cfb4-137">String</span></span>|<span data-ttu-id="2cfb4-138">O nome do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-138">The intune device's name.</span></span>|
|<span data-ttu-id="2cfb4-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="2cfb4-139">serialNumber</span></span>|<span data-ttu-id="2cfb4-140">String</span><span class="sxs-lookup"><span data-stu-id="2cfb4-140">String</span></span>|<span data-ttu-id="2cfb4-141">O número de série do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-141">The intune device's serial number.</span></span>|
|<span data-ttu-id="2cfb4-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="2cfb4-142">manufacturer</span></span>|<span data-ttu-id="2cfb4-143">String</span><span class="sxs-lookup"><span data-stu-id="2cfb4-143">String</span></span>|<span data-ttu-id="2cfb4-144">O fabricante do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-144">The intune device's manufacturer.</span></span>|
|<span data-ttu-id="2cfb4-145">modelo</span><span class="sxs-lookup"><span data-stu-id="2cfb4-145">model</span></span>|<span data-ttu-id="2cfb4-146">String</span><span class="sxs-lookup"><span data-stu-id="2cfb4-146">String</span></span>|<span data-ttu-id="2cfb4-147">O modelo do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-147">The intune device's model.</span></span>|
|<span data-ttu-id="2cfb4-148">managedBy</span><span class="sxs-lookup"><span data-stu-id="2cfb4-148">managedBy</span></span>|<span data-ttu-id="2cfb4-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cfb4-149">String</span></span>|<span data-ttu-id="2cfb4-150">O dispositivo do intune é gerenciado por.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-150">The intune device's managed by.</span></span>|
|<span data-ttu-id="2cfb4-151">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="2cfb4-151">autoPilotRegistered</span></span>|<span data-ttu-id="2cfb4-152">Booleano</span><span class="sxs-lookup"><span data-stu-id="2cfb4-152">Boolean</span></span>|<span data-ttu-id="2cfb4-153">O piloto automático do dispositivo intuneRegistered.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-153">The intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="2cfb4-154">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="2cfb4-154">autoPilotProfileAssigned</span></span>|<span data-ttu-id="2cfb4-155">Booleano</span><span class="sxs-lookup"><span data-stu-id="2cfb4-155">Boolean</span></span>|<span data-ttu-id="2cfb4-156">O autopilotProfileAssigned do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-156">The intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="2cfb4-157">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="2cfb4-157">azureAdRegistered</span></span>|[<span data-ttu-id="2cfb4-158">azureAdRegisteredState</span><span class="sxs-lookup"><span data-stu-id="2cfb4-158">azureAdRegisteredState</span></span>](../resources/intune-devices-azureadregisteredstate.md)|<span data-ttu-id="2cfb4-159">O dispositivo do intune é azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-159">The intune device's azureAdRegistered.</span></span> <span data-ttu-id="2cfb4-160">Os valores possíveis são: `no`, `yes`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-160">Possible values are: `no`, `yes`, `unknown`.</span></span>|
|<span data-ttu-id="2cfb4-161">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="2cfb4-161">azureAdJoinType</span></span>|<span data-ttu-id="2cfb4-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cfb4-162">String</span></span>|<span data-ttu-id="2cfb4-163">O azure Ad joinType do dispositivo do intune.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-163">The intune device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="2cfb4-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cfb4-164">Response</span></span>
<span data-ttu-id="2cfb4-165">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-165">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cfb4-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cfb4-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cfb4-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cfb4-167">Request</span></span>
<span data-ttu-id="2cfb4-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
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

### <a name="response"></a><span data-ttu-id="2cfb4-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cfb4-169">Response</span></span>
<span data-ttu-id="2cfb4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cfb4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




