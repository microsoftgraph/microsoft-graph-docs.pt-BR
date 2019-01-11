---
title: Get deviceComplianceDeviceStatus
description: Ler propriedades e relações do objeto deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2f2ed86505d552e57dd7f83c09acae6c819dbf7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850964"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="8db47-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8db47-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="8db47-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8db47-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8db47-105">Ler propriedades e relações do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8db47-105">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8db47-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8db47-106">Prerequisites</span></span>
<span data-ttu-id="8db47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8db47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8db47-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8db47-109">Permission type</span></span>|<span data-ttu-id="8db47-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8db47-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8db47-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8db47-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8db47-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8db47-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8db47-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8db47-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8db47-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8db47-114">Not supported.</span></span>|
|<span data-ttu-id="8db47-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8db47-115">Application</span></span>|<span data-ttu-id="8db47-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8db47-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8db47-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8db47-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8db47-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8db47-118">Optional query parameters</span></span>
<span data-ttu-id="8db47-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8db47-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8db47-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8db47-120">Request headers</span></span>
|<span data-ttu-id="8db47-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8db47-121">Header</span></span>|<span data-ttu-id="8db47-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8db47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8db47-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8db47-123">Authorization</span></span>|<span data-ttu-id="8db47-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8db47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8db47-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8db47-125">Accept</span></span>|<span data-ttu-id="8db47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8db47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8db47-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8db47-127">Request body</span></span>
<span data-ttu-id="8db47-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8db47-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8db47-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8db47-129">Response</span></span>
<span data-ttu-id="8db47-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8db47-130">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8db47-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8db47-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8db47-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8db47-132">Request</span></span>
<span data-ttu-id="8db47-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8db47-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8db47-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8db47-134">Response</span></span>
<span data-ttu-id="8db47-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8db47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



