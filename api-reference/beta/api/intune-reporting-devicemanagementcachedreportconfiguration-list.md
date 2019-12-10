---
title: Listar deviceManagementCachedReportConfigurations
description: Listar Propriedades e relações dos objetos deviceManagementCachedReportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3dfe5ed51f1f6842fe18a8dd7a6c56f02c34826b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940359"
---
# <a name="list-devicemanagementcachedreportconfigurations"></a><span data-ttu-id="16fed-103">Listar deviceManagementCachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="16fed-103">List deviceManagementCachedReportConfigurations</span></span>

> <span data-ttu-id="16fed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16fed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16fed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16fed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16fed-106">Listar Propriedades e relações dos objetos [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="16fed-106">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16fed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16fed-107">Prerequisites</span></span>
<span data-ttu-id="16fed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16fed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16fed-110">Permission type</span></span>|<span data-ttu-id="16fed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16fed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16fed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16fed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16fed-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="16fed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="16fed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16fed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16fed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16fed-115">Not supported.</span></span>|
|<span data-ttu-id="16fed-116">Application</span><span class="sxs-lookup"><span data-stu-id="16fed-116">Application</span></span>|<span data-ttu-id="16fed-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="16fed-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16fed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16fed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="16fed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16fed-119">Request headers</span></span>
|<span data-ttu-id="16fed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16fed-120">Header</span></span>|<span data-ttu-id="16fed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16fed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16fed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16fed-122">Authorization</span></span>|<span data-ttu-id="16fed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16fed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16fed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16fed-124">Accept</span></span>|<span data-ttu-id="16fed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16fed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16fed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16fed-126">Request body</span></span>
<span data-ttu-id="16fed-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16fed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16fed-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="16fed-128">Response</span></span>
<span data-ttu-id="16fed-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16fed-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16fed-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16fed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="16fed-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16fed-131">Request</span></span>
<span data-ttu-id="16fed-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16fed-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
```

### <a name="response"></a><span data-ttu-id="16fed-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="16fed-133">Response</span></span>
<span data-ttu-id="16fed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16fed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 519

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
      "status": "notStarted",
      "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
    }
  ]
}
```





