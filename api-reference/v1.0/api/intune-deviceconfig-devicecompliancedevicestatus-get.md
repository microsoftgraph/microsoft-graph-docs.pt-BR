---
title: Get deviceComplianceDeviceStatus
description: Ler propriedades e relações do objeto deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42d62f8562f151573aac1c2ad417373bd41d97f8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760654"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="8df8c-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8df8c-103">Get deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="8df8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8df8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8df8c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8df8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8df8c-106">Ler propriedades e relações do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8df8c-106">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8df8c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8df8c-107">Prerequisites</span></span>
<span data-ttu-id="8df8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df8c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8df8c-110">Permission type</span></span>|<span data-ttu-id="8df8c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8df8c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df8c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8df8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8df8c-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df8c-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8df8c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8df8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df8c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8df8c-115">Not supported.</span></span>|
|<span data-ttu-id="8df8c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8df8c-116">Application</span></span>|<span data-ttu-id="8df8c-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df8c-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df8c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8df8c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8df8c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8df8c-119">Optional query parameters</span></span>
<span data-ttu-id="8df8c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8df8c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8df8c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8df8c-121">Request headers</span></span>
|<span data-ttu-id="8df8c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8df8c-122">Header</span></span>|<span data-ttu-id="8df8c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8df8c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8df8c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8df8c-124">Authorization</span></span>|<span data-ttu-id="8df8c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8df8c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8df8c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8df8c-126">Accept</span></span>|<span data-ttu-id="8df8c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8df8c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df8c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8df8c-128">Request body</span></span>
<span data-ttu-id="8df8c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8df8c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8df8c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df8c-130">Response</span></span>
<span data-ttu-id="8df8c-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8df8c-131">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df8c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8df8c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8df8c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8df8c-133">Request</span></span>
<span data-ttu-id="8df8c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8df8c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8df8c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df8c-135">Response</span></span>
<span data-ttu-id="8df8c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8df8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




