---
title: Obter managedDeviceMobileAppConfigurationDeviceSummary
description: Ler propriedades e relações do objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a31e8ac2b3c87d38a0f1e2892eab295f0f691cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014001"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="6a662-103">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6a662-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="6a662-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a662-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a662-105">Ler propriedades e relações do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6a662-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a662-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a662-106">Prerequisites</span></span>
<span data-ttu-id="6a662-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a662-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a662-109">Permission type</span></span>|<span data-ttu-id="6a662-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a662-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a662-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a662-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a662-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a662-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6a662-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a662-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a662-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a662-114">Not supported.</span></span>|
|<span data-ttu-id="6a662-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a662-115">Application</span></span>|<span data-ttu-id="6a662-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a662-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a662-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a662-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a662-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a662-118">Optional query parameters</span></span>
<span data-ttu-id="6a662-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a662-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a662-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a662-120">Request headers</span></span>
|<span data-ttu-id="6a662-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a662-121">Header</span></span>|<span data-ttu-id="6a662-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a662-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a662-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a662-123">Authorization</span></span>|<span data-ttu-id="6a662-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a662-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a662-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a662-125">Accept</span></span>|<span data-ttu-id="6a662-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a662-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a662-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a662-127">Request body</span></span>
<span data-ttu-id="6a662-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a662-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a662-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a662-129">Response</span></span>
<span data-ttu-id="6a662-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a662-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a662-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a662-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a662-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a662-132">Request</span></span>
<span data-ttu-id="6a662-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a662-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="6a662-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a662-134">Response</span></span>
<span data-ttu-id="6a662-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a662-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



