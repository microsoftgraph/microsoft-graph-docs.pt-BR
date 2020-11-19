---
title: Listar deviceManagementCachedReportConfigurations
description: Listar Propriedades e relações dos objetos deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82ece3ebdb8a62d5e399ee05ee82853859e75699
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210547"
---
# <a name="list-devicemanagementcachedreportconfigurations"></a><span data-ttu-id="1bd60-103">Listar deviceManagementCachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="1bd60-103">List deviceManagementCachedReportConfigurations</span></span>

<span data-ttu-id="1bd60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bd60-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bd60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bd60-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bd60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd60-107">Listar Propriedades e relações dos objetos [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1bd60-107">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bd60-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bd60-108">Prerequisites</span></span>
<span data-ttu-id="1bd60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd60-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bd60-111">Permission type</span></span>|<span data-ttu-id="1bd60-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bd60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bd60-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bd60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bd60-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="1bd60-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1bd60-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bd60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bd60-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bd60-116">Not supported.</span></span>|
|<span data-ttu-id="1bd60-117">Application</span><span class="sxs-lookup"><span data-stu-id="1bd60-117">Application</span></span>|<span data-ttu-id="1bd60-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="1bd60-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bd60-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1bd60-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd60-120">Request headers</span></span>
|<span data-ttu-id="1bd60-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bd60-121">Header</span></span>|<span data-ttu-id="1bd60-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1bd60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bd60-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bd60-123">Authorization</span></span>|<span data-ttu-id="1bd60-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bd60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bd60-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bd60-125">Accept</span></span>|<span data-ttu-id="1bd60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bd60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bd60-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd60-127">Request body</span></span>
<span data-ttu-id="1bd60-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bd60-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bd60-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd60-129">Response</span></span>
<span data-ttu-id="1bd60-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd60-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bd60-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bd60-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bd60-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd60-132">Request</span></span>
<span data-ttu-id="1bd60-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bd60-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
```

### <a name="response"></a><span data-ttu-id="1bd60-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd60-134">Response</span></span>
<span data-ttu-id="1bd60-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bd60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




