---
title: Listar deviceManagementReportSchedules
description: Listar Propriedades e relações dos objetos deviceManagementReportSchedule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ec0473da4ffa8c9808e5595695d397a3d4dabf9d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459068"
---
# <a name="list-devicemanagementreportschedules"></a><span data-ttu-id="29ddc-103">Listar deviceManagementReportSchedules</span><span class="sxs-lookup"><span data-stu-id="29ddc-103">List deviceManagementReportSchedules</span></span>

<span data-ttu-id="29ddc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29ddc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29ddc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29ddc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29ddc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29ddc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29ddc-107">Listar Propriedades e relações dos objetos [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="29ddc-107">List properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29ddc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29ddc-108">Prerequisites</span></span>
<span data-ttu-id="29ddc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29ddc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29ddc-111">Permission type</span></span>|<span data-ttu-id="29ddc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29ddc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29ddc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29ddc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29ddc-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="29ddc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="29ddc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29ddc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29ddc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29ddc-116">Not supported.</span></span>|
|<span data-ttu-id="29ddc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29ddc-117">Application</span></span>|<span data-ttu-id="29ddc-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="29ddc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29ddc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29ddc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="29ddc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29ddc-120">Request headers</span></span>
|<span data-ttu-id="29ddc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29ddc-121">Header</span></span>|<span data-ttu-id="29ddc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29ddc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29ddc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29ddc-123">Authorization</span></span>|<span data-ttu-id="29ddc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29ddc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29ddc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29ddc-125">Accept</span></span>|<span data-ttu-id="29ddc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29ddc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29ddc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29ddc-127">Request body</span></span>
<span data-ttu-id="29ddc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29ddc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29ddc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="29ddc-129">Response</span></span>
<span data-ttu-id="29ddc-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29ddc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29ddc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29ddc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="29ddc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29ddc-132">Request</span></span>
<span data-ttu-id="29ddc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29ddc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
```

### <a name="response"></a><span data-ttu-id="29ddc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="29ddc-134">Response</span></span>
<span data-ttu-id="29ddc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29ddc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 701

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
      "id": "00bb9785-9785-00bb-8597-bb008597bb00",
      "reportScheduleName": "Report Schedule Name value",
      "subject": "Subject value",
      "emails": [
        "Emails value"
      ],
      "recurrence": "daily",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
      "userId": "User Id value",
      "reportName": "Report Name value",
      "filter": "Filter value",
      "select": [
        "Select value"
      ],
      "orderBy": [
        "Order By value"
      ],
      "format": "pdf"
    }
  ]
}
```





