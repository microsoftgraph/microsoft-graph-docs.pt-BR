---
title: Listar unmanagedDeviceDiscoveryTasks
description: Listar propriedades e relações dos objetos unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a11c278328d859a1c8769fbbe1ee99012fe27e29
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134750"
---
# <a name="list-unmanageddevicediscoverytasks"></a><span data-ttu-id="f2fef-103">Listar unmanagedDeviceDiscoveryTasks</span><span class="sxs-lookup"><span data-stu-id="f2fef-103">List unmanagedDeviceDiscoveryTasks</span></span>

<span data-ttu-id="f2fef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2fef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2fef-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2fef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2fef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2fef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2fef-107">Listar propriedades e relações dos [objetos unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="f2fef-107">List properties and relationships of the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2fef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2fef-108">Prerequisites</span></span>
<span data-ttu-id="f2fef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2fef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2fef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2fef-111">Permission type</span></span>|<span data-ttu-id="f2fef-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2fef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2fef-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2fef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2fef-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fef-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2fef-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2fef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2fef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2fef-116">Not supported.</span></span>|
|<span data-ttu-id="f2fef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2fef-117">Application</span></span>|<span data-ttu-id="f2fef-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fef-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2fef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2fef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="f2fef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2fef-120">Request headers</span></span>
|<span data-ttu-id="f2fef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2fef-121">Header</span></span>|<span data-ttu-id="f2fef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2fef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2fef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2fef-123">Authorization</span></span>|<span data-ttu-id="f2fef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2fef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2fef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2fef-125">Accept</span></span>|<span data-ttu-id="f2fef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2fef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2fef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2fef-127">Request body</span></span>
<span data-ttu-id="f2fef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2fef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2fef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2fef-129">Response</span></span>
<span data-ttu-id="f2fef-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2fef-130">If successful, this method returns a `200 OK` response code and a collection of [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2fef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2fef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2fef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2fef-132">Request</span></span>
<span data-ttu-id="f2fef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2fef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a><span data-ttu-id="f2fef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2fef-134">Response</span></span>
<span data-ttu-id="f2fef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2fef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1214

{
  "value": [
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
  ]
}
```




