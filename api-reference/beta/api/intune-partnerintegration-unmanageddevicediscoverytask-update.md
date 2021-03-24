---
title: Atualizar unmanagedDeviceDiscoveryTask
description: Atualize as propriedades de um objeto unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 87722cb838dcc46d7275c8de3530a7d1792b6e3d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141775"
---
# <a name="update-unmanageddevicediscoverytask"></a><span data-ttu-id="a4e44-103">Atualizar unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="a4e44-103">Update unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="a4e44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4e44-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4e44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4e44-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4e44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4e44-107">Atualize as propriedades de [um objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-107">Update the properties of a [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4e44-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4e44-108">Prerequisites</span></span>
<span data-ttu-id="a4e44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4e44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e44-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4e44-111">Permission type</span></span>|<span data-ttu-id="a4e44-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4e44-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4e44-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4e44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4e44-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e44-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4e44-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4e44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4e44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4e44-116">Not supported.</span></span>|
|<span data-ttu-id="a4e44-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4e44-117">Application</span></span>|<span data-ttu-id="a4e44-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e44-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4e44-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4e44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="a4e44-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e44-120">Request headers</span></span>
|<span data-ttu-id="a4e44-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4e44-121">Header</span></span>|<span data-ttu-id="a4e44-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a4e44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4e44-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4e44-123">Authorization</span></span>|<span data-ttu-id="a4e44-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4e44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4e44-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4e44-125">Accept</span></span>|<span data-ttu-id="a4e44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4e44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4e44-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e44-127">Request body</span></span>
<span data-ttu-id="a4e44-128">No corpo da solicitação, fornece uma representação JSON para o [objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-128">In the request body, supply a JSON representation for the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

<span data-ttu-id="a4e44-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).</span><span class="sxs-lookup"><span data-stu-id="a4e44-129">The following table shows the properties that are required when you create the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).</span></span>

|<span data-ttu-id="a4e44-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4e44-130">Property</span></span>|<span data-ttu-id="a4e44-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4e44-131">Type</span></span>|<span data-ttu-id="a4e44-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4e44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4e44-133">id</span><span class="sxs-lookup"><span data-stu-id="a4e44-133">id</span></span>|<span data-ttu-id="a4e44-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e44-134">String</span></span>|<span data-ttu-id="a4e44-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a4e44-135">The entity key.</span></span> <span data-ttu-id="a4e44-136">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a4e44-137">displayName</span></span>|<span data-ttu-id="a4e44-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e44-138">String</span></span>|<span data-ttu-id="a4e44-139">O nome.</span><span class="sxs-lookup"><span data-stu-id="a4e44-139">The name.</span></span> <span data-ttu-id="a4e44-140">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-141">descrição</span><span class="sxs-lookup"><span data-stu-id="a4e44-141">description</span></span>|<span data-ttu-id="a4e44-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e44-142">String</span></span>|<span data-ttu-id="a4e44-143">A descrição.</span><span class="sxs-lookup"><span data-stu-id="a4e44-143">The description.</span></span> <span data-ttu-id="a4e44-144">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4e44-145">createdDateTime</span></span>|<span data-ttu-id="a4e44-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4e44-146">DateTimeOffset</span></span>|<span data-ttu-id="a4e44-147">A data criada.</span><span class="sxs-lookup"><span data-stu-id="a4e44-147">The created date.</span></span> <span data-ttu-id="a4e44-148">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="a4e44-149">dueDateTime</span></span>|<span data-ttu-id="a4e44-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4e44-150">DateTimeOffset</span></span>|<span data-ttu-id="a4e44-151">A data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="a4e44-151">The due date.</span></span> <span data-ttu-id="a4e44-152">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-153">category</span><span class="sxs-lookup"><span data-stu-id="a4e44-153">category</span></span>|[<span data-ttu-id="a4e44-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="a4e44-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="a4e44-155">A categoria.</span><span class="sxs-lookup"><span data-stu-id="a4e44-155">The category.</span></span> <span data-ttu-id="a4e44-156">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="a4e44-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="a4e44-157">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="a4e44-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="a4e44-158">prioridade</span><span class="sxs-lookup"><span data-stu-id="a4e44-158">priority</span></span>|[<span data-ttu-id="a4e44-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="a4e44-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="a4e44-160">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="a4e44-160">The priority.</span></span> <span data-ttu-id="a4e44-161">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="a4e44-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="a4e44-162">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="a4e44-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="a4e44-163">criador</span><span class="sxs-lookup"><span data-stu-id="a4e44-163">creator</span></span>|<span data-ttu-id="a4e44-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e44-164">String</span></span>|<span data-ttu-id="a4e44-165">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="a4e44-165">The email address of the creator.</span></span> <span data-ttu-id="a4e44-166">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="a4e44-167">creatorNotes</span></span>|<span data-ttu-id="a4e44-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e44-168">String</span></span>|<span data-ttu-id="a4e44-169">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="a4e44-169">Notes from the creator.</span></span> <span data-ttu-id="a4e44-170">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="a4e44-171">assignedTo</span></span>|<span data-ttu-id="a4e44-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e44-172">String</span></span>|<span data-ttu-id="a4e44-173">O nome ou o email do administrador ao que essa tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="a4e44-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="a4e44-174">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="a4e44-175">status</span><span class="sxs-lookup"><span data-stu-id="a4e44-175">status</span></span>|[<span data-ttu-id="a4e44-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="a4e44-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="a4e44-177">O status.</span><span class="sxs-lookup"><span data-stu-id="a4e44-177">The status.</span></span> <span data-ttu-id="a4e44-178">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="a4e44-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="a4e44-179">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="a4e44-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="a4e44-180">unmanagedDevices</span><span class="sxs-lookup"><span data-stu-id="a4e44-180">unmanagedDevices</span></span>|<span data-ttu-id="a4e44-181">[Coleção unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a4e44-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) collection</span></span>|<span data-ttu-id="a4e44-182">Dispositivos nãomanageados descobertos na rede.</span><span class="sxs-lookup"><span data-stu-id="a4e44-182">Unmanaged devices discovered in the network.</span></span>|



## <a name="response"></a><span data-ttu-id="a4e44-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4e44-183">Response</span></span>
<span data-ttu-id="a4e44-184">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4e44-184">If successful, this method returns a `200 OK` response code and an updated [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4e44-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4e44-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4e44-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e44-186">Request</span></span>
<span data-ttu-id="a4e44-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4e44-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4e44-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4e44-188">Response</span></span>
<span data-ttu-id="a4e44-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4e44-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




