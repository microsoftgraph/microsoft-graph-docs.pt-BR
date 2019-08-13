---
title: Get deviceComplianceDeviceStatus
description: Ler propriedades e relações do objeto deviceComplianceDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d7d0684c5d9935642cccdbfd22cc73b9d6d6698
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310875"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="8a51a-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8a51a-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="8a51a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a51a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a51a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a51a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a51a-106">Ler propriedades e relações do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8a51a-106">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a51a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a51a-107">Prerequisites</span></span>
<span data-ttu-id="8a51a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a51a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a51a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a51a-110">Permission type</span></span>|<span data-ttu-id="8a51a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a51a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a51a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a51a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a51a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a51a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8a51a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a51a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a51a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a51a-115">Not supported.</span></span>|
|<span data-ttu-id="8a51a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a51a-116">Application</span></span>|<span data-ttu-id="8a51a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a51a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a51a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a51a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a51a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8a51a-119">Optional query parameters</span></span>
<span data-ttu-id="8a51a-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8a51a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a51a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a51a-121">Request headers</span></span>
|<span data-ttu-id="8a51a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a51a-122">Header</span></span>|<span data-ttu-id="8a51a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8a51a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a51a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a51a-124">Authorization</span></span>|<span data-ttu-id="8a51a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a51a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a51a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a51a-126">Accept</span></span>|<span data-ttu-id="8a51a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8a51a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a51a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a51a-128">Request body</span></span>
<span data-ttu-id="8a51a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a51a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a51a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a51a-130">Response</span></span>
<span data-ttu-id="8a51a-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a51a-131">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a51a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a51a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a51a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a51a-133">Request</span></span>
<span data-ttu-id="8a51a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a51a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8a51a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a51a-135">Response</span></span>
<span data-ttu-id="8a51a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a51a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```






