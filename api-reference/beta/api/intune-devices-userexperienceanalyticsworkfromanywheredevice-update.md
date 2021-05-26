---
title: Atualizar userExperienceAnalyticsWorkFromAnywhereDevice
description: Atualize as propriedades de um objeto userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5fb8eb16af3a192c6def8088866f7891f7afa85
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665025"
---
# <a name="update-userexperienceanalyticsworkfromanywheredevice"></a><span data-ttu-id="32324-103">Atualizar userExperienceAnalyticsWorkFromAnywhereDevice</span><span class="sxs-lookup"><span data-stu-id="32324-103">Update userExperienceAnalyticsWorkFromAnywhereDevice</span></span>

<span data-ttu-id="32324-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32324-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32324-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32324-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32324-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32324-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32324-107">Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="32324-107">Update the properties of a [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32324-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32324-108">Prerequisites</span></span>
<span data-ttu-id="32324-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32324-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32324-111">Permission type</span></span>|<span data-ttu-id="32324-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32324-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32324-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32324-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32324-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="32324-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32324-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32324-116">Not supported.</span></span>|
|<span data-ttu-id="32324-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32324-117">Application</span></span>|<span data-ttu-id="32324-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32324-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32324-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="32324-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32324-120">Request headers</span></span>
|<span data-ttu-id="32324-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32324-121">Header</span></span>|<span data-ttu-id="32324-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32324-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32324-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32324-123">Authorization</span></span>|<span data-ttu-id="32324-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32324-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32324-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32324-125">Accept</span></span>|<span data-ttu-id="32324-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32324-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32324-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32324-127">Request body</span></span>
<span data-ttu-id="32324-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="32324-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

<span data-ttu-id="32324-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md).</span><span class="sxs-lookup"><span data-stu-id="32324-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md).</span></span>

|<span data-ttu-id="32324-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32324-130">Property</span></span>|<span data-ttu-id="32324-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="32324-131">Type</span></span>|<span data-ttu-id="32324-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="32324-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32324-133">id</span><span class="sxs-lookup"><span data-stu-id="32324-133">id</span></span>|<span data-ttu-id="32324-134">String</span><span class="sxs-lookup"><span data-stu-id="32324-134">String</span></span>|<span data-ttu-id="32324-135">O identificador exclusivo da análise de experiência do usuário funciona em qualquer dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-135">The unique identifier of the user experience analytics work from anywhere device.</span></span>|
|<span data-ttu-id="32324-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="32324-136">deviceName</span></span>|<span data-ttu-id="32324-137">String</span><span class="sxs-lookup"><span data-stu-id="32324-137">String</span></span>|<span data-ttu-id="32324-138">O trabalho do nome do dispositivo em qualquer lugar.</span><span class="sxs-lookup"><span data-stu-id="32324-138">The work from anywhere device's name.</span></span>|
|<span data-ttu-id="32324-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="32324-139">serialNumber</span></span>|<span data-ttu-id="32324-140">String</span><span class="sxs-lookup"><span data-stu-id="32324-140">String</span></span>|<span data-ttu-id="32324-141">A experiência do usuário funciona de qualquer lugar do número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-141">The user experience work from anywhere device's serial number.</span></span>|
|<span data-ttu-id="32324-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="32324-142">manufacturer</span></span>|<span data-ttu-id="32324-143">String</span><span class="sxs-lookup"><span data-stu-id="32324-143">String</span></span>|<span data-ttu-id="32324-144">A experiência do usuário funciona de qualquer fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-144">The user experience work from anywhere device's manufacturer.</span></span>|
|<span data-ttu-id="32324-145">modelo</span><span class="sxs-lookup"><span data-stu-id="32324-145">model</span></span>|<span data-ttu-id="32324-146">String</span><span class="sxs-lookup"><span data-stu-id="32324-146">String</span></span>|<span data-ttu-id="32324-147">A experiência do usuário funciona de qualquer lugar do modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-147">The user experience work from anywhere device's model.</span></span>|
|<span data-ttu-id="32324-148">propriedade</span><span class="sxs-lookup"><span data-stu-id="32324-148">ownership</span></span>|<span data-ttu-id="32324-149">String</span><span class="sxs-lookup"><span data-stu-id="32324-149">String</span></span>|<span data-ttu-id="32324-150">A experiência do usuário funciona de qualquer lugar da propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-150">The user experience work from anywhere device's ownership.</span></span>|
|<span data-ttu-id="32324-151">managedBy</span><span class="sxs-lookup"><span data-stu-id="32324-151">managedBy</span></span>|<span data-ttu-id="32324-152">String</span><span class="sxs-lookup"><span data-stu-id="32324-152">String</span></span>|<span data-ttu-id="32324-153">A experiência do usuário funciona de qualquer lugar do agente de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-153">The user experience work from anywhere management agent of the device.</span></span>|
|<span data-ttu-id="32324-154">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="32324-154">autoPilotRegistered</span></span>|<span data-ttu-id="32324-155">Booleano</span><span class="sxs-lookup"><span data-stu-id="32324-155">Boolean</span></span>|<span data-ttu-id="32324-156">A experiência do usuário funciona em qualquer lugar do piloto automático do dispositivo intuneRegistered.</span><span class="sxs-lookup"><span data-stu-id="32324-156">The user experience work from anywhere intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="32324-157">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="32324-157">autoPilotProfileAssigned</span></span>|<span data-ttu-id="32324-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="32324-158">Boolean</span></span>|<span data-ttu-id="32324-159">A análise da experiência do usuário funciona em qualquer lugar do autopilotProfileAssigned do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="32324-159">The user experience analytics work from anywhere intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="32324-160">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="32324-160">azureAdRegistered</span></span>|<span data-ttu-id="32324-161">Booleano</span><span class="sxs-lookup"><span data-stu-id="32324-161">Boolean</span></span>|<span data-ttu-id="32324-162">A experiência do usuário funciona de qualquer lugar do dispositivo azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="32324-162">The user experience work from anywhere device's azureAdRegistered.</span></span>|
|<span data-ttu-id="32324-163">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="32324-163">azureAdDeviceId</span></span>|<span data-ttu-id="32324-164">String</span><span class="sxs-lookup"><span data-stu-id="32324-164">String</span></span>|<span data-ttu-id="32324-165">A experiência do usuário funciona em qualquer lugar do Azure Ad device Id.</span><span class="sxs-lookup"><span data-stu-id="32324-165">The user experience work from anywhere azure Ad device Id.</span></span>|
|<span data-ttu-id="32324-166">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="32324-166">azureAdJoinType</span></span>|<span data-ttu-id="32324-167">String</span><span class="sxs-lookup"><span data-stu-id="32324-167">String</span></span>|<span data-ttu-id="32324-168">A experiência do usuário funciona de qualquer lugar do azure Ad joinType do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-168">The user experience work from anywhere device's azure Ad joinType.</span></span>|
|<span data-ttu-id="32324-169">osDescription</span><span class="sxs-lookup"><span data-stu-id="32324-169">osDescription</span></span>|<span data-ttu-id="32324-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32324-170">String</span></span>|<span data-ttu-id="32324-171">A experiência do usuário funciona de qualquer lugar da Descrição do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-171">The user experience work from anywhere device's OS Description.</span></span>|
|<span data-ttu-id="32324-172">osVersion</span><span class="sxs-lookup"><span data-stu-id="32324-172">osVersion</span></span>|<span data-ttu-id="32324-173">String</span><span class="sxs-lookup"><span data-stu-id="32324-173">String</span></span>|<span data-ttu-id="32324-174">A experiência do usuário funciona de qualquer lugar da versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32324-174">The user experience work from anywhere device's OS Version.</span></span>|



## <a name="response"></a><span data-ttu-id="32324-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="32324-175">Response</span></span>
<span data-ttu-id="32324-176">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32324-176">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32324-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32324-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="32324-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32324-178">Request</span></span>
<span data-ttu-id="32324-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32324-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
Content-type: application/json
Content-length: 585

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value"
}
```

### <a name="response"></a><span data-ttu-id="32324-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="32324-180">Response</span></span>
<span data-ttu-id="32324-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32324-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 634

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value"
}
```




