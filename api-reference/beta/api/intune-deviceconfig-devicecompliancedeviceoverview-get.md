---
title: Acessar deviceComplianceDeviceOverview
description: Leia as propriedades e as relações do objeto deviceComplianceDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1a349f1c7fee26081743908a8d759278e07474d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310889"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="f3475-103">Acessar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f3475-103">Get deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="f3475-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3475-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3475-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3475-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3475-106">Leia as propriedades e as relações do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f3475-106">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3475-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3475-107">Prerequisites</span></span>
<span data-ttu-id="f3475-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3475-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3475-110">Permission type</span></span>|<span data-ttu-id="f3475-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3475-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3475-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3475-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3475-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3475-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f3475-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3475-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3475-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3475-115">Not supported.</span></span>|
|<span data-ttu-id="f3475-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3475-116">Application</span></span>|<span data-ttu-id="f3475-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3475-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3475-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3475-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3475-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f3475-119">Optional query parameters</span></span>
<span data-ttu-id="f3475-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f3475-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3475-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3475-121">Request headers</span></span>
|<span data-ttu-id="f3475-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3475-122">Header</span></span>|<span data-ttu-id="f3475-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f3475-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3475-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3475-124">Authorization</span></span>|<span data-ttu-id="f3475-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3475-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3475-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3475-126">Accept</span></span>|<span data-ttu-id="f3475-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f3475-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3475-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3475-128">Request body</span></span>
<span data-ttu-id="f3475-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3475-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3475-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3475-130">Response</span></span>
<span data-ttu-id="f3475-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3475-131">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3475-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3475-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3475-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3475-133">Request</span></span>
<span data-ttu-id="f3475-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3475-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="f3475-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3475-135">Response</span></span>
<span data-ttu-id="f3475-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3475-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 432

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
    "id": "886f167b-167b-886f-7b16-6f887b166f88",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```






