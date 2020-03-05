---
title: Obter deviceManagementExportJob
description: Leia as propriedades e as relações do objeto deviceManagementExportJob.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 693868a810bc09547e333d20cb6d6c1e899474cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459215"
---
# <a name="get-devicemanagementexportjob"></a><span data-ttu-id="22019-103">Obter deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="22019-103">Get deviceManagementExportJob</span></span>

<span data-ttu-id="22019-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22019-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22019-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22019-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22019-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22019-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22019-107">Leia as propriedades e as relações do objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .</span><span class="sxs-lookup"><span data-stu-id="22019-107">Read properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22019-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22019-108">Prerequisites</span></span>
<span data-ttu-id="22019-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22019-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22019-111">Permission type</span></span>|<span data-ttu-id="22019-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22019-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22019-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22019-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22019-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="22019-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="22019-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22019-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22019-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22019-116">Not supported.</span></span>|
|<span data-ttu-id="22019-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22019-117">Application</span></span>|<span data-ttu-id="22019-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="22019-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22019-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22019-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22019-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22019-120">Optional query parameters</span></span>
<span data-ttu-id="22019-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22019-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22019-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22019-122">Request headers</span></span>
|<span data-ttu-id="22019-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22019-123">Header</span></span>|<span data-ttu-id="22019-124">Valor</span><span class="sxs-lookup"><span data-stu-id="22019-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22019-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="22019-125">Authorization</span></span>|<span data-ttu-id="22019-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22019-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22019-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22019-127">Accept</span></span>|<span data-ttu-id="22019-128">application/json</span><span class="sxs-lookup"><span data-stu-id="22019-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22019-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22019-129">Request body</span></span>
<span data-ttu-id="22019-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22019-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22019-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="22019-131">Response</span></span>
<span data-ttu-id="22019-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22019-132">If successful, this method returns a `200 OK` response code and [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22019-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22019-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="22019-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22019-134">Request</span></span>
<span data-ttu-id="22019-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22019-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

### <a name="response"></a><span data-ttu-id="22019-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="22019-136">Response</span></span>
<span data-ttu-id="22019-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22019-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "value": {
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
}
```





