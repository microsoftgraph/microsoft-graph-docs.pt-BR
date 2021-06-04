---
title: Obter managedDeviceMobileAppConfigurationDeviceSummary
description: Ler propriedades e relações do objeto managedDeviceMobileAppConfigurationDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 628594276e0cf271c42881549d1d7275eb0805b8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754221"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="6644a-103">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6644a-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="6644a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6644a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6644a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6644a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6644a-106">Ler propriedades e relações do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6644a-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6644a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6644a-107">Prerequisites</span></span>
<span data-ttu-id="6644a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6644a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6644a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6644a-110">Permission type</span></span>|<span data-ttu-id="6644a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6644a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6644a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6644a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6644a-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6644a-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6644a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6644a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6644a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6644a-115">Not supported.</span></span>|
|<span data-ttu-id="6644a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6644a-116">Application</span></span>|<span data-ttu-id="6644a-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6644a-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6644a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6644a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6644a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6644a-119">Optional query parameters</span></span>
<span data-ttu-id="6644a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6644a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6644a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6644a-121">Request headers</span></span>
|<span data-ttu-id="6644a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6644a-122">Header</span></span>|<span data-ttu-id="6644a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6644a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6644a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6644a-124">Authorization</span></span>|<span data-ttu-id="6644a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6644a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6644a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6644a-126">Accept</span></span>|<span data-ttu-id="6644a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6644a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6644a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6644a-128">Request body</span></span>
<span data-ttu-id="6644a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6644a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6644a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6644a-130">Response</span></span>
<span data-ttu-id="6644a-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6644a-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6644a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6644a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6644a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6644a-133">Request</span></span>
<span data-ttu-id="6644a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6644a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="6644a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6644a-135">Response</span></span>
<span data-ttu-id="6644a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6644a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




