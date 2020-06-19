---
title: Listar deviceManagementCachedReportConfigurations
description: Listar Propriedades e relações dos objetos deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9d0a982bc598fc9e42b684dcda0e84a2d38e0aa
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791346"
---
# <a name="list-devicemanagementcachedreportconfigurations"></a><span data-ttu-id="4f90e-103">Listar deviceManagementCachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="4f90e-103">List deviceManagementCachedReportConfigurations</span></span>

<span data-ttu-id="4f90e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f90e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f90e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f90e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f90e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f90e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f90e-107">Listar Propriedades e relações dos objetos [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4f90e-107">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f90e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f90e-108">Prerequisites</span></span>
<span data-ttu-id="4f90e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4f90e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4f90e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f90e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f90e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f90e-111">Permission type</span></span>|<span data-ttu-id="4f90e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f90e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f90e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f90e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f90e-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="4f90e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4f90e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f90e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f90e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f90e-116">Not supported.</span></span>|
|<span data-ttu-id="4f90e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f90e-117">Application</span></span>|<span data-ttu-id="4f90e-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="4f90e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f90e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f90e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f90e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f90e-120">Request headers</span></span>
|<span data-ttu-id="4f90e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f90e-121">Header</span></span>|<span data-ttu-id="4f90e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f90e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f90e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f90e-123">Authorization</span></span>|<span data-ttu-id="4f90e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f90e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f90e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f90e-125">Accept</span></span>|<span data-ttu-id="4f90e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f90e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f90e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f90e-127">Request body</span></span>
<span data-ttu-id="4f90e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f90e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f90e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f90e-129">Response</span></span>
<span data-ttu-id="4f90e-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f90e-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f90e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f90e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f90e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f90e-132">Request</span></span>
<span data-ttu-id="4f90e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f90e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
```

### <a name="response"></a><span data-ttu-id="4f90e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f90e-134">Response</span></span>
<span data-ttu-id="4f90e-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="4f90e-135">Here is an example of the response.</span></span> <span data-ttu-id="4f90e-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4f90e-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4f90e-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4f90e-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 556

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
      "id": "46947722-7722-4694-2277-944622779446",
      "reportName": "Report Name value",
      "filter": "Filter value",
      "select": [
        "Select value"
      ],
      "orderBy": [
        "Order By value"
      ],
      "metadata": "Metadata value",
      "status": "notStarted",
      "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
    }
  ]
}
```



