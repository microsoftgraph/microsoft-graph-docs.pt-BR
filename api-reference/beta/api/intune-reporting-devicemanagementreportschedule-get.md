---
title: Obter deviceManagementReportSchedule
description: Leia as propriedades e as relações do objeto deviceManagementReportSchedule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aec39ce5376b0db3178ea150f6da9bd9b7fce9e9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537181"
---
# <a name="get-devicemanagementreportschedule"></a><span data-ttu-id="38ec1-103">Obter deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="38ec1-103">Get deviceManagementReportSchedule</span></span>

> <span data-ttu-id="38ec1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38ec1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38ec1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38ec1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38ec1-106">Leia as propriedades e as relações do objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="38ec1-106">Read properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38ec1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38ec1-107">Prerequisites</span></span>
<span data-ttu-id="38ec1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38ec1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38ec1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38ec1-110">Permission type</span></span>|<span data-ttu-id="38ec1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38ec1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38ec1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38ec1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38ec1-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="38ec1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="38ec1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38ec1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38ec1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38ec1-115">Not supported.</span></span>|
|<span data-ttu-id="38ec1-116">Application</span><span class="sxs-lookup"><span data-stu-id="38ec1-116">Application</span></span>|<span data-ttu-id="38ec1-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="38ec1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38ec1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38ec1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38ec1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38ec1-119">Optional query parameters</span></span>
<span data-ttu-id="38ec1-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38ec1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38ec1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38ec1-121">Request headers</span></span>
|<span data-ttu-id="38ec1-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38ec1-122">Header</span></span>|<span data-ttu-id="38ec1-123">Valor</span><span class="sxs-lookup"><span data-stu-id="38ec1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38ec1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="38ec1-124">Authorization</span></span>|<span data-ttu-id="38ec1-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38ec1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38ec1-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38ec1-126">Accept</span></span>|<span data-ttu-id="38ec1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="38ec1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38ec1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38ec1-128">Request body</span></span>
<span data-ttu-id="38ec1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38ec1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38ec1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ec1-130">Response</span></span>
<span data-ttu-id="38ec1-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38ec1-131">If successful, this method returns a `200 OK` response code and [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ec1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38ec1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="38ec1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38ec1-133">Request</span></span>
<span data-ttu-id="38ec1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38ec1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

### <a name="response"></a><span data-ttu-id="38ec1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ec1-135">Response</span></span>
<span data-ttu-id="38ec1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38ec1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 647

{
  "value": {
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
}
```






