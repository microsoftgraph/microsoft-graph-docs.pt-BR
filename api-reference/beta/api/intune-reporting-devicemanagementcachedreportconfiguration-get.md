---
title: Obter deviceManagementCachedReportConfiguration
description: Leia as propriedades e as relações do objeto deviceManagementCachedReportConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c26784e17a0a42ddbe3c12e5e9052e83f0fc34bc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801457"
---
# <a name="get-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="04213-103">Obter deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="04213-103">Get deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="04213-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04213-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04213-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04213-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04213-106">Leia as propriedades e as relações do objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="04213-106">Read properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04213-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04213-107">Prerequisites</span></span>
<span data-ttu-id="04213-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04213-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04213-110">Permission type</span></span>|<span data-ttu-id="04213-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04213-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04213-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04213-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04213-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="04213-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="04213-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04213-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04213-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04213-115">Not supported.</span></span>|
|<span data-ttu-id="04213-116">Application</span><span class="sxs-lookup"><span data-stu-id="04213-116">Application</span></span>|<span data-ttu-id="04213-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="04213-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04213-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04213-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04213-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04213-119">Optional query parameters</span></span>
<span data-ttu-id="04213-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04213-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04213-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04213-121">Request headers</span></span>
|<span data-ttu-id="04213-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04213-122">Header</span></span>|<span data-ttu-id="04213-123">Valor</span><span class="sxs-lookup"><span data-stu-id="04213-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04213-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="04213-124">Authorization</span></span>|<span data-ttu-id="04213-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04213-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04213-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04213-126">Accept</span></span>|<span data-ttu-id="04213-127">application/json</span><span class="sxs-lookup"><span data-stu-id="04213-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04213-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04213-128">Request body</span></span>
<span data-ttu-id="04213-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04213-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04213-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="04213-130">Response</span></span>
<span data-ttu-id="04213-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04213-131">If successful, this method returns a `200 OK` response code and [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04213-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04213-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="04213-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04213-133">Request</span></span>
<span data-ttu-id="04213-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04213-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

### <a name="response"></a><span data-ttu-id="04213-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="04213-135">Response</span></span>
<span data-ttu-id="04213-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04213-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 479

{
  "value": {
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
}
```




