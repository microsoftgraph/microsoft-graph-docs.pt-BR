---
title: Atualizar unmanagedDeviceDiscoveryTask
description: Atualizar as propriedades de um objeto unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7908c6a79cba41312d4f8ac850c78d32076c21b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160137"
---
# <a name="update-unmanageddevicediscoverytask"></a><span data-ttu-id="76915-103">Atualizar unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="76915-103">Update unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="76915-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76915-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76915-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76915-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76915-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76915-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76915-107">Atualizar as propriedades de [um objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-107">Update the properties of a [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76915-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76915-108">Prerequisites</span></span>
<span data-ttu-id="76915-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76915-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76915-111">Permission type</span></span>|<span data-ttu-id="76915-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76915-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76915-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76915-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76915-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76915-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76915-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76915-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76915-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76915-116">Not supported.</span></span>|
|<span data-ttu-id="76915-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76915-117">Application</span></span>|<span data-ttu-id="76915-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76915-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76915-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76915-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="76915-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76915-120">Request headers</span></span>
|<span data-ttu-id="76915-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76915-121">Header</span></span>|<span data-ttu-id="76915-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76915-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76915-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76915-123">Authorization</span></span>|<span data-ttu-id="76915-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76915-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76915-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76915-125">Accept</span></span>|<span data-ttu-id="76915-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76915-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76915-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76915-127">Request body</span></span>
<span data-ttu-id="76915-128">No corpo da solicitação, fornece uma representação JSON do [objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-128">In the request body, supply a JSON representation for the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

<span data-ttu-id="76915-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).</span><span class="sxs-lookup"><span data-stu-id="76915-129">The following table shows the properties that are required when you create the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).</span></span>

|<span data-ttu-id="76915-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76915-130">Property</span></span>|<span data-ttu-id="76915-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76915-131">Type</span></span>|<span data-ttu-id="76915-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76915-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76915-133">id</span><span class="sxs-lookup"><span data-stu-id="76915-133">id</span></span>|<span data-ttu-id="76915-134">String</span><span class="sxs-lookup"><span data-stu-id="76915-134">String</span></span>|<span data-ttu-id="76915-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76915-135">The entity key.</span></span> <span data-ttu-id="76915-136">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-137">displayName</span><span class="sxs-lookup"><span data-stu-id="76915-137">displayName</span></span>|<span data-ttu-id="76915-138">String</span><span class="sxs-lookup"><span data-stu-id="76915-138">String</span></span>|<span data-ttu-id="76915-139">O nome.</span><span class="sxs-lookup"><span data-stu-id="76915-139">The name.</span></span> <span data-ttu-id="76915-140">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-141">description</span><span class="sxs-lookup"><span data-stu-id="76915-141">description</span></span>|<span data-ttu-id="76915-142">String</span><span class="sxs-lookup"><span data-stu-id="76915-142">String</span></span>|<span data-ttu-id="76915-143">A descrição.</span><span class="sxs-lookup"><span data-stu-id="76915-143">The description.</span></span> <span data-ttu-id="76915-144">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76915-145">createdDateTime</span></span>|<span data-ttu-id="76915-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76915-146">DateTimeOffset</span></span>|<span data-ttu-id="76915-147">A data de criação.</span><span class="sxs-lookup"><span data-stu-id="76915-147">The created date.</span></span> <span data-ttu-id="76915-148">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="76915-149">dueDateTime</span></span>|<span data-ttu-id="76915-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76915-150">DateTimeOffset</span></span>|<span data-ttu-id="76915-151">A data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="76915-151">The due date.</span></span> <span data-ttu-id="76915-152">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-153">category</span><span class="sxs-lookup"><span data-stu-id="76915-153">category</span></span>|[<span data-ttu-id="76915-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="76915-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="76915-155">A categoria.</span><span class="sxs-lookup"><span data-stu-id="76915-155">The category.</span></span> <span data-ttu-id="76915-156">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="76915-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="76915-157">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="76915-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="76915-158">prioridade</span><span class="sxs-lookup"><span data-stu-id="76915-158">priority</span></span>|[<span data-ttu-id="76915-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="76915-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="76915-160">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="76915-160">The priority.</span></span> <span data-ttu-id="76915-161">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="76915-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="76915-162">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="76915-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="76915-163">criador</span><span class="sxs-lookup"><span data-stu-id="76915-163">creator</span></span>|<span data-ttu-id="76915-164">String</span><span class="sxs-lookup"><span data-stu-id="76915-164">String</span></span>|<span data-ttu-id="76915-165">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="76915-165">The email address of the creator.</span></span> <span data-ttu-id="76915-166">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="76915-167">creatorNotes</span></span>|<span data-ttu-id="76915-168">String</span><span class="sxs-lookup"><span data-stu-id="76915-168">String</span></span>|<span data-ttu-id="76915-169">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="76915-169">Notes from the creator.</span></span> <span data-ttu-id="76915-170">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="76915-171">assignedTo</span></span>|<span data-ttu-id="76915-172">String</span><span class="sxs-lookup"><span data-stu-id="76915-172">String</span></span>|<span data-ttu-id="76915-173">O nome ou email do administrador ao que essa tarefa foi atribuída.</span><span class="sxs-lookup"><span data-stu-id="76915-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="76915-174">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="76915-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="76915-175">status</span><span class="sxs-lookup"><span data-stu-id="76915-175">status</span></span>|[<span data-ttu-id="76915-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="76915-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="76915-177">O status.</span><span class="sxs-lookup"><span data-stu-id="76915-177">The status.</span></span> <span data-ttu-id="76915-178">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="76915-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="76915-179">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="76915-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="76915-180">unmanagedDevices</span><span class="sxs-lookup"><span data-stu-id="76915-180">unmanagedDevices</span></span>|<span data-ttu-id="76915-181">[Coleção unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="76915-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) collection</span></span>|<span data-ttu-id="76915-182">Dispositivos não-manageados descobertos na rede.</span><span class="sxs-lookup"><span data-stu-id="76915-182">Unmanaged devices discovered in the network.</span></span>|



## <a name="response"></a><span data-ttu-id="76915-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="76915-183">Response</span></span>
<span data-ttu-id="76915-184">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76915-184">If successful, this method returns a `200 OK` response code and an updated [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76915-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76915-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="76915-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76915-186">Request</span></span>
<span data-ttu-id="76915-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76915-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 961

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="76915-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="76915-188">Response</span></span>
<span data-ttu-id="76915-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76915-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "id": "6caa2ba0-2ba0-6caa-a02b-aa6ca02baa6c",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```




