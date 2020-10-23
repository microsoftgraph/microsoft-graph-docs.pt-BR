---
title: Listar deviceManagementExportJobs
description: Listar Propriedades e relações dos objetos deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d7c45ea5fede157ce372db1c94ed9ae28a38ce8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698243"
---
# <a name="list-devicemanagementexportjobs"></a><span data-ttu-id="f3cae-103">Listar deviceManagementExportJobs</span><span class="sxs-lookup"><span data-stu-id="f3cae-103">List deviceManagementExportJobs</span></span>

<span data-ttu-id="f3cae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3cae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3cae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3cae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3cae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3cae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3cae-107">Listar Propriedades e relações dos objetos [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="f3cae-107">List properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3cae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3cae-108">Prerequisites</span></span>
<span data-ttu-id="f3cae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3cae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3cae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3cae-111">Permission type</span></span>|<span data-ttu-id="f3cae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3cae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3cae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3cae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3cae-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="f3cae-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f3cae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3cae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3cae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3cae-116">Not supported.</span></span>|
|<span data-ttu-id="f3cae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3cae-117">Application</span></span>|<span data-ttu-id="f3cae-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="f3cae-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3cae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3cae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="f3cae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3cae-120">Request headers</span></span>
|<span data-ttu-id="f3cae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3cae-121">Header</span></span>|<span data-ttu-id="f3cae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f3cae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3cae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3cae-123">Authorization</span></span>|<span data-ttu-id="f3cae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3cae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3cae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3cae-125">Accept</span></span>|<span data-ttu-id="f3cae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3cae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3cae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3cae-127">Request body</span></span>
<span data-ttu-id="f3cae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3cae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3cae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3cae-129">Response</span></span>
<span data-ttu-id="f3cae-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3cae-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3cae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3cae-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3cae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3cae-132">Request</span></span>
<span data-ttu-id="f3cae-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3cae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
```

### <a name="response"></a><span data-ttu-id="f3cae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3cae-134">Response</span></span>
<span data-ttu-id="f3cae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3cae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 538

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExportJob",
      "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
      "reportName": "Report Name value",
      "filter": "Filter value",
      "select": [
        "Select value"
      ],
      "format": "pdf",
      "snapshotId": "Snapshot Id value",
      "status": "notStarted",
      "url": "Url value",
      "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
    }
  ]
}
```





