---
title: Criar userExperienceAnalyticsNotAutopilotReadyDevice
description: Crie um novo objeto userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1473c0a856636dc5373239c1bed4c2caed9ea78b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865219"
---
# <a name="create-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="88639-103">Criar userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="88639-103">Create userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="88639-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88639-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88639-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88639-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88639-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88639-107">Crie um novo [objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="88639-107">Create a new [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88639-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88639-108">Prerequisites</span></span>
<span data-ttu-id="88639-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88639-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88639-111">Permission type</span></span>|<span data-ttu-id="88639-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88639-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88639-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88639-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88639-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88639-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88639-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88639-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88639-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88639-116">Not supported.</span></span>|
|<span data-ttu-id="88639-117">Application</span><span class="sxs-lookup"><span data-stu-id="88639-117">Application</span></span>|<span data-ttu-id="88639-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88639-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88639-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88639-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a><span data-ttu-id="88639-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88639-120">Request headers</span></span>
|<span data-ttu-id="88639-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88639-121">Header</span></span>|<span data-ttu-id="88639-122">Valor</span><span class="sxs-lookup"><span data-stu-id="88639-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88639-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88639-123">Authorization</span></span>|<span data-ttu-id="88639-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88639-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88639-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88639-125">Accept</span></span>|<span data-ttu-id="88639-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88639-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88639-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88639-127">Request body</span></span>
<span data-ttu-id="88639-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="88639-128">In the request body, supply a JSON representation for the userExperienceAnalyticsNotAutopilotReadyDevice object.</span></span>

<span data-ttu-id="88639-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="88639-129">The following table shows the properties that are required when you create the userExperienceAnalyticsNotAutopilotReadyDevice.</span></span>

|<span data-ttu-id="88639-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88639-130">Property</span></span>|<span data-ttu-id="88639-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="88639-131">Type</span></span>|<span data-ttu-id="88639-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="88639-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88639-133">id</span><span class="sxs-lookup"><span data-stu-id="88639-133">id</span></span>|<span data-ttu-id="88639-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88639-134">String</span></span>|<span data-ttu-id="88639-135">O identificador exclusivo do dispositivo intune de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="88639-135">The unique identifier of the user experience analytics intune device.</span></span>|
|<span data-ttu-id="88639-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="88639-136">deviceName</span></span>|<span data-ttu-id="88639-137">String</span><span class="sxs-lookup"><span data-stu-id="88639-137">String</span></span>|<span data-ttu-id="88639-138">O nome do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="88639-138">The intune device's name.</span></span>|
|<span data-ttu-id="88639-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="88639-139">serialNumber</span></span>|<span data-ttu-id="88639-140">String</span><span class="sxs-lookup"><span data-stu-id="88639-140">String</span></span>|<span data-ttu-id="88639-141">O número de série do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="88639-141">The intune device's serial number.</span></span>|
|<span data-ttu-id="88639-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="88639-142">manufacturer</span></span>|<span data-ttu-id="88639-143">String</span><span class="sxs-lookup"><span data-stu-id="88639-143">String</span></span>|<span data-ttu-id="88639-144">O fabricante do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="88639-144">The intune device's manufacturer.</span></span>|
|<span data-ttu-id="88639-145">modelo</span><span class="sxs-lookup"><span data-stu-id="88639-145">model</span></span>|<span data-ttu-id="88639-146">String</span><span class="sxs-lookup"><span data-stu-id="88639-146">String</span></span>|<span data-ttu-id="88639-147">O modelo do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="88639-147">The intune device's model.</span></span>|
|<span data-ttu-id="88639-148">managedBy</span><span class="sxs-lookup"><span data-stu-id="88639-148">managedBy</span></span>|<span data-ttu-id="88639-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="88639-149">String</span></span>|<span data-ttu-id="88639-150">O dispositivo do intune é gerenciado por.</span><span class="sxs-lookup"><span data-stu-id="88639-150">The intune device's managed by.</span></span>|
|<span data-ttu-id="88639-151">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="88639-151">autoPilotRegistered</span></span>|<span data-ttu-id="88639-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="88639-152">Boolean</span></span>|<span data-ttu-id="88639-153">O piloto automático do dispositivo intuneRegistered.</span><span class="sxs-lookup"><span data-stu-id="88639-153">The intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="88639-154">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="88639-154">autoPilotProfileAssigned</span></span>|<span data-ttu-id="88639-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="88639-155">Boolean</span></span>|<span data-ttu-id="88639-156">O autopilotProfileAssigned do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="88639-156">The intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="88639-157">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="88639-157">azureAdRegistered</span></span>|<span data-ttu-id="88639-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="88639-158">Boolean</span></span>|<span data-ttu-id="88639-159">O dispositivo do intune é azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="88639-159">The intune device's azureAdRegistered.</span></span>|
|<span data-ttu-id="88639-160">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="88639-160">azureAdJoinType</span></span>|<span data-ttu-id="88639-161">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="88639-161">String</span></span>|<span data-ttu-id="88639-162">O azure Ad joinType do dispositivo do intune.</span><span class="sxs-lookup"><span data-stu-id="88639-162">The intune device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="88639-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="88639-163">Response</span></span>
<span data-ttu-id="88639-164">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88639-164">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88639-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88639-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="88639-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88639-166">Request</span></span>
<span data-ttu-id="88639-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88639-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="88639-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="88639-168">Response</span></span>
<span data-ttu-id="88639-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88639-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 470

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
  "azureAdRegistered": true,
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




