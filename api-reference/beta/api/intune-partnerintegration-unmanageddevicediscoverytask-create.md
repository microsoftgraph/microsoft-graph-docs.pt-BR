---
title: Criar unmanagedDeviceDiscoveryTask
description: Crie um novo objeto unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 032b1e19e72dae2a30f125ab5c030098a23d8ad6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134799"
---
# <a name="create-unmanageddevicediscoverytask"></a><span data-ttu-id="29869-103">Criar unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="29869-103">Create unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="29869-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29869-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29869-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29869-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29869-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29869-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29869-107">Crie um novo [objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-107">Create a new [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29869-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29869-108">Prerequisites</span></span>
<span data-ttu-id="29869-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29869-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29869-111">Permission type</span></span>|<span data-ttu-id="29869-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29869-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29869-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29869-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29869-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29869-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29869-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29869-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29869-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29869-116">Not supported.</span></span>|
|<span data-ttu-id="29869-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29869-117">Application</span></span>|<span data-ttu-id="29869-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29869-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29869-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29869-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="29869-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29869-120">Request headers</span></span>
|<span data-ttu-id="29869-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29869-121">Header</span></span>|<span data-ttu-id="29869-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29869-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29869-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29869-123">Authorization</span></span>|<span data-ttu-id="29869-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29869-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29869-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29869-125">Accept</span></span>|<span data-ttu-id="29869-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29869-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29869-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29869-127">Request body</span></span>
<span data-ttu-id="29869-128">No corpo da solicitação, fornece uma representação JSON para o objeto unmanagedDeviceDiscoveryTask.</span><span class="sxs-lookup"><span data-stu-id="29869-128">In the request body, supply a JSON representation for the unmanagedDeviceDiscoveryTask object.</span></span>

<span data-ttu-id="29869-129">A tabela a seguir mostra as propriedades que são necessárias ao criar unmanagedDeviceDiscoveryTask.</span><span class="sxs-lookup"><span data-stu-id="29869-129">The following table shows the properties that are required when you create the unmanagedDeviceDiscoveryTask.</span></span>

|<span data-ttu-id="29869-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29869-130">Property</span></span>|<span data-ttu-id="29869-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29869-131">Type</span></span>|<span data-ttu-id="29869-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29869-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29869-133">id</span><span class="sxs-lookup"><span data-stu-id="29869-133">id</span></span>|<span data-ttu-id="29869-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29869-134">String</span></span>|<span data-ttu-id="29869-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="29869-135">The entity key.</span></span> <span data-ttu-id="29869-136">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-137">displayName</span><span class="sxs-lookup"><span data-stu-id="29869-137">displayName</span></span>|<span data-ttu-id="29869-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29869-138">String</span></span>|<span data-ttu-id="29869-139">O nome.</span><span class="sxs-lookup"><span data-stu-id="29869-139">The name.</span></span> <span data-ttu-id="29869-140">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-141">descrição</span><span class="sxs-lookup"><span data-stu-id="29869-141">description</span></span>|<span data-ttu-id="29869-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29869-142">String</span></span>|<span data-ttu-id="29869-143">A descrição.</span><span class="sxs-lookup"><span data-stu-id="29869-143">The description.</span></span> <span data-ttu-id="29869-144">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29869-145">createdDateTime</span></span>|<span data-ttu-id="29869-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29869-146">DateTimeOffset</span></span>|<span data-ttu-id="29869-147">A data criada.</span><span class="sxs-lookup"><span data-stu-id="29869-147">The created date.</span></span> <span data-ttu-id="29869-148">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="29869-149">dueDateTime</span></span>|<span data-ttu-id="29869-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29869-150">DateTimeOffset</span></span>|<span data-ttu-id="29869-151">A data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="29869-151">The due date.</span></span> <span data-ttu-id="29869-152">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-153">category</span><span class="sxs-lookup"><span data-stu-id="29869-153">category</span></span>|[<span data-ttu-id="29869-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="29869-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="29869-155">A categoria.</span><span class="sxs-lookup"><span data-stu-id="29869-155">The category.</span></span> <span data-ttu-id="29869-156">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="29869-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="29869-157">Os valores possíveis são: `unknown` e `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="29869-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="29869-158">prioridade</span><span class="sxs-lookup"><span data-stu-id="29869-158">priority</span></span>|[<span data-ttu-id="29869-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="29869-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="29869-160">A prioridade.</span><span class="sxs-lookup"><span data-stu-id="29869-160">The priority.</span></span> <span data-ttu-id="29869-161">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="29869-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="29869-162">Os valores possíveis são: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="29869-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="29869-163">criador</span><span class="sxs-lookup"><span data-stu-id="29869-163">creator</span></span>|<span data-ttu-id="29869-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29869-164">String</span></span>|<span data-ttu-id="29869-165">O endereço de email do criador.</span><span class="sxs-lookup"><span data-stu-id="29869-165">The email address of the creator.</span></span> <span data-ttu-id="29869-166">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="29869-167">creatorNotes</span></span>|<span data-ttu-id="29869-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29869-168">String</span></span>|<span data-ttu-id="29869-169">Observações do criador.</span><span class="sxs-lookup"><span data-stu-id="29869-169">Notes from the creator.</span></span> <span data-ttu-id="29869-170">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="29869-171">assignedTo</span></span>|<span data-ttu-id="29869-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29869-172">String</span></span>|<span data-ttu-id="29869-173">O nome ou o email do administrador ao que essa tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="29869-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="29869-174">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="29869-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="29869-175">status</span><span class="sxs-lookup"><span data-stu-id="29869-175">status</span></span>|[<span data-ttu-id="29869-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="29869-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="29869-177">O status.</span><span class="sxs-lookup"><span data-stu-id="29869-177">The status.</span></span> <span data-ttu-id="29869-178">Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="29869-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="29869-179">Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="29869-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="29869-180">unmanagedDevices</span><span class="sxs-lookup"><span data-stu-id="29869-180">unmanagedDevices</span></span>|<span data-ttu-id="29869-181">[Coleção unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="29869-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) collection</span></span>|<span data-ttu-id="29869-182">Dispositivos nãomanageados descobertos na rede.</span><span class="sxs-lookup"><span data-stu-id="29869-182">Unmanaged devices discovered in the network.</span></span>|



## <a name="response"></a><span data-ttu-id="29869-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="29869-183">Response</span></span>
<span data-ttu-id="29869-184">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29869-184">If successful, this method returns a `201 Created` response code and a [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29869-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29869-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="29869-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29869-186">Request</span></span>
<span data-ttu-id="29869-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29869-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
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

### <a name="response"></a><span data-ttu-id="29869-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="29869-188">Response</span></span>
<span data-ttu-id="29869-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29869-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




