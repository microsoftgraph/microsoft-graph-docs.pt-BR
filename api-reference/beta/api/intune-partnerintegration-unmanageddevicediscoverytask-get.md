---
title: Obter unmanagedDeviceDiscoveryTask
description: Leia propriedades e relações do objeto unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8770ee1d0393f1b484fdba32bba883d5fd2e37bd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134757"
---
# <a name="get-unmanageddevicediscoverytask"></a><span data-ttu-id="76160-103">Obter unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="76160-103">Get unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="76160-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76160-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76160-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76160-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76160-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76160-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76160-107">Leia propriedades e relações do [objeto unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="76160-107">Read properties and relationships of the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76160-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76160-108">Prerequisites</span></span>
<span data-ttu-id="76160-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76160-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76160-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76160-111">Permission type</span></span>|<span data-ttu-id="76160-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76160-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76160-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76160-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76160-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76160-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76160-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76160-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76160-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76160-116">Not supported.</span></span>|
|<span data-ttu-id="76160-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76160-117">Application</span></span>|<span data-ttu-id="76160-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76160-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76160-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76160-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76160-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="76160-120">Optional query parameters</span></span>
<span data-ttu-id="76160-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="76160-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76160-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76160-122">Request headers</span></span>
|<span data-ttu-id="76160-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76160-123">Header</span></span>|<span data-ttu-id="76160-124">Valor</span><span class="sxs-lookup"><span data-stu-id="76160-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76160-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="76160-125">Authorization</span></span>|<span data-ttu-id="76160-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76160-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76160-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76160-127">Accept</span></span>|<span data-ttu-id="76160-128">application/json</span><span class="sxs-lookup"><span data-stu-id="76160-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76160-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76160-129">Request body</span></span>
<span data-ttu-id="76160-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76160-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76160-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="76160-131">Response</span></span>
<span data-ttu-id="76160-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76160-132">If successful, this method returns a `200 OK` response code and [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76160-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76160-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="76160-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76160-134">Request</span></span>
<span data-ttu-id="76160-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76160-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

### <a name="response"></a><span data-ttu-id="76160-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="76160-136">Response</span></span>
<span data-ttu-id="76160-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76160-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1144

{
  "value": {
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
}
```




