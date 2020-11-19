---
title: Obter deviceManagementReportSchedule
description: Leia as propriedades e as relações do objeto deviceManagementReportSchedule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df1ac1267dec76892647217b211c4309c9f17a76
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257615"
---
# <a name="get-devicemanagementreportschedule"></a><span data-ttu-id="8aa91-103">Obter deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="8aa91-103">Get deviceManagementReportSchedule</span></span>

<span data-ttu-id="8aa91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aa91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8aa91-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8aa91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8aa91-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8aa91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8aa91-107">Leia as propriedades e as relações do objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="8aa91-107">Read properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8aa91-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8aa91-108">Prerequisites</span></span>
<span data-ttu-id="8aa91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aa91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aa91-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aa91-111">Permission type</span></span>|<span data-ttu-id="8aa91-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8aa91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aa91-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aa91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8aa91-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="8aa91-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8aa91-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aa91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aa91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aa91-116">Not supported.</span></span>|
|<span data-ttu-id="8aa91-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aa91-117">Application</span></span>|<span data-ttu-id="8aa91-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="8aa91-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aa91-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aa91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8aa91-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8aa91-120">Optional query parameters</span></span>
<span data-ttu-id="8aa91-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8aa91-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8aa91-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa91-122">Request headers</span></span>
|<span data-ttu-id="8aa91-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8aa91-123">Header</span></span>|<span data-ttu-id="8aa91-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8aa91-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8aa91-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aa91-125">Authorization</span></span>|<span data-ttu-id="8aa91-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8aa91-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8aa91-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8aa91-127">Accept</span></span>|<span data-ttu-id="8aa91-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8aa91-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aa91-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa91-129">Request body</span></span>
<span data-ttu-id="8aa91-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8aa91-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aa91-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aa91-131">Response</span></span>
<span data-ttu-id="8aa91-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aa91-132">If successful, this method returns a `200 OK` response code and [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aa91-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8aa91-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8aa91-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa91-134">Request</span></span>
<span data-ttu-id="8aa91-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aa91-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

### <a name="response"></a><span data-ttu-id="8aa91-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aa91-136">Response</span></span>
<span data-ttu-id="8aa91-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8aa91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




