---
title: Criar userExperienceAnalyticsWorkFromAnywhereDevice
description: Crie um novo objeto userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cd4db22f691935d53b85eded268650ab0bc12b4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868341"
---
# <a name="create-userexperienceanalyticsworkfromanywheredevice"></a><span data-ttu-id="33aa4-103">Criar userExperienceAnalyticsWorkFromAnywhereDevice</span><span class="sxs-lookup"><span data-stu-id="33aa4-103">Create userExperienceAnalyticsWorkFromAnywhereDevice</span></span>

<span data-ttu-id="33aa4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33aa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33aa4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33aa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33aa4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33aa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33aa4-107">Crie um novo [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="33aa4-107">Create a new [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33aa4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33aa4-108">Prerequisites</span></span>
<span data-ttu-id="33aa4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33aa4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33aa4-111">Permission type</span></span>|<span data-ttu-id="33aa4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33aa4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33aa4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33aa4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33aa4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33aa4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="33aa4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33aa4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33aa4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33aa4-116">Not supported.</span></span>|
|<span data-ttu-id="33aa4-117">Application</span><span class="sxs-lookup"><span data-stu-id="33aa4-117">Application</span></span>|<span data-ttu-id="33aa4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33aa4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33aa4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33aa4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a><span data-ttu-id="33aa4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33aa4-120">Request headers</span></span>
|<span data-ttu-id="33aa4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33aa4-121">Header</span></span>|<span data-ttu-id="33aa4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33aa4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33aa4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33aa4-123">Authorization</span></span>|<span data-ttu-id="33aa4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33aa4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33aa4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33aa4-125">Accept</span></span>|<span data-ttu-id="33aa4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33aa4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33aa4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33aa4-127">Request body</span></span>
<span data-ttu-id="33aa4-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsWorkFromAnywhereDevice.</span><span class="sxs-lookup"><span data-stu-id="33aa4-128">In the request body, supply a JSON representation for the userExperienceAnalyticsWorkFromAnywhereDevice object.</span></span>

<span data-ttu-id="33aa4-129">A tabela a seguir mostra as propriedades necessárias ao criar o userExperienceAnalyticsWorkFromAnywhereDevice.</span><span class="sxs-lookup"><span data-stu-id="33aa4-129">The following table shows the properties that are required when you create the userExperienceAnalyticsWorkFromAnywhereDevice.</span></span>

|<span data-ttu-id="33aa4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33aa4-130">Property</span></span>|<span data-ttu-id="33aa4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33aa4-131">Type</span></span>|<span data-ttu-id="33aa4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33aa4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33aa4-133">id</span><span class="sxs-lookup"><span data-stu-id="33aa4-133">id</span></span>|<span data-ttu-id="33aa4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33aa4-134">String</span></span>|<span data-ttu-id="33aa4-135">O identificador exclusivo da análise de experiência do usuário funciona em qualquer dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33aa4-135">The unique identifier of the user experience analytics work from anywhere device.</span></span>|
|<span data-ttu-id="33aa4-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="33aa4-136">deviceName</span></span>|<span data-ttu-id="33aa4-137">String</span><span class="sxs-lookup"><span data-stu-id="33aa4-137">String</span></span>|<span data-ttu-id="33aa4-138">O trabalho do nome do dispositivo em qualquer lugar.</span><span class="sxs-lookup"><span data-stu-id="33aa4-138">The work from anywhere device's name.</span></span>|
|<span data-ttu-id="33aa4-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="33aa4-139">serialNumber</span></span>|<span data-ttu-id="33aa4-140">String</span><span class="sxs-lookup"><span data-stu-id="33aa4-140">String</span></span>|<span data-ttu-id="33aa4-141">A experiência do usuário funciona de qualquer lugar do número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33aa4-141">The user experience work from anywhere device's serial number.</span></span>|
|<span data-ttu-id="33aa4-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="33aa4-142">manufacturer</span></span>|<span data-ttu-id="33aa4-143">String</span><span class="sxs-lookup"><span data-stu-id="33aa4-143">String</span></span>|<span data-ttu-id="33aa4-144">A experiência do usuário funciona de qualquer fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33aa4-144">The user experience work from anywhere device's manufacturer.</span></span>|
|<span data-ttu-id="33aa4-145">modelo</span><span class="sxs-lookup"><span data-stu-id="33aa4-145">model</span></span>|<span data-ttu-id="33aa4-146">String</span><span class="sxs-lookup"><span data-stu-id="33aa4-146">String</span></span>|<span data-ttu-id="33aa4-147">A experiência do usuário funciona de qualquer lugar do modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33aa4-147">The user experience work from anywhere device's model.</span></span>|
|<span data-ttu-id="33aa4-148">propriedade</span><span class="sxs-lookup"><span data-stu-id="33aa4-148">ownership</span></span>|<span data-ttu-id="33aa4-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="33aa4-149">String</span></span>|<span data-ttu-id="33aa4-150">A experiência do usuário funciona de qualquer lugar da propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33aa4-150">The user experience work from anywhere device's ownership.</span></span>|
|<span data-ttu-id="33aa4-151">managedBy</span><span class="sxs-lookup"><span data-stu-id="33aa4-151">managedBy</span></span>|<span data-ttu-id="33aa4-152">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="33aa4-152">String</span></span>|<span data-ttu-id="33aa4-153">A experiência do usuário funciona de qualquer lugar do agente de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33aa4-153">The user experience work from anywhere management agent of the device.</span></span>|
|<span data-ttu-id="33aa4-154">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="33aa4-154">autoPilotRegistered</span></span>|<span data-ttu-id="33aa4-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="33aa4-155">Boolean</span></span>|<span data-ttu-id="33aa4-156">A experiência do usuário funciona em qualquer lugar do piloto automático do dispositivo intuneRegistered.</span><span class="sxs-lookup"><span data-stu-id="33aa4-156">The user experience work from anywhere intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="33aa4-157">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="33aa4-157">autoPilotProfileAssigned</span></span>|<span data-ttu-id="33aa4-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="33aa4-158">Boolean</span></span>|<span data-ttu-id="33aa4-159">A análise da experiência do usuário funciona em qualquer lugar do autopilotProfileAssigned do dispositivo intune.</span><span class="sxs-lookup"><span data-stu-id="33aa4-159">The user experience analytics work from anywhere intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="33aa4-160">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="33aa4-160">azureAdRegistered</span></span>|<span data-ttu-id="33aa4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="33aa4-161">Boolean</span></span>|<span data-ttu-id="33aa4-162">A experiência do usuário funciona de qualquer lugar do dispositivo azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="33aa4-162">The user experience work from anywhere device's azureAdRegistered.</span></span>|
|<span data-ttu-id="33aa4-163">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="33aa4-163">azureAdDeviceId</span></span>|<span data-ttu-id="33aa4-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="33aa4-164">String</span></span>|<span data-ttu-id="33aa4-165">A experiência do usuário funciona em qualquer lugar do Azure Ad device Id.</span><span class="sxs-lookup"><span data-stu-id="33aa4-165">The user experience work from anywhere azure Ad device Id.</span></span>|
|<span data-ttu-id="33aa4-166">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="33aa4-166">azureAdJoinType</span></span>|<span data-ttu-id="33aa4-167">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="33aa4-167">String</span></span>|<span data-ttu-id="33aa4-168">A experiência do usuário funciona de qualquer lugar do azure Ad joinType do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="33aa4-168">The user experience work from anywhere device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="33aa4-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="33aa4-169">Response</span></span>
<span data-ttu-id="33aa4-170">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33aa4-170">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33aa4-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33aa4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="33aa4-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33aa4-172">Request</span></span>
<span data-ttu-id="33aa4-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33aa4-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
Content-type: application/json
Content-length: 505

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
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="33aa4-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="33aa4-174">Response</span></span>
<span data-ttu-id="33aa4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33aa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 554

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
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




