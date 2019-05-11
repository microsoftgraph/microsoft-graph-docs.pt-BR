---
title: Listar deviceComplianceDeviceStatuses
description: Listar propriedades e relações dos objetos deviceComplianceDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28b3e89ef999b11554a6d6a01be7d758d095f19f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927941"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="c20ed-103">Listar deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c20ed-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="c20ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c20ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c20ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c20ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c20ed-106">Listar propriedades e relações dos objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c20ed-106">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c20ed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c20ed-107">Prerequisites</span></span>
<span data-ttu-id="c20ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c20ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c20ed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c20ed-110">Permission type</span></span>|<span data-ttu-id="c20ed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c20ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c20ed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c20ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c20ed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c20ed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c20ed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c20ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c20ed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c20ed-115">Not supported.</span></span>|
|<span data-ttu-id="c20ed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c20ed-116">Application</span></span>|<span data-ttu-id="c20ed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c20ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c20ed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c20ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c20ed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c20ed-119">Request headers</span></span>
|<span data-ttu-id="c20ed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c20ed-120">Header</span></span>|<span data-ttu-id="c20ed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c20ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c20ed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c20ed-122">Authorization</span></span>|<span data-ttu-id="c20ed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c20ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c20ed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c20ed-124">Accept</span></span>|<span data-ttu-id="c20ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c20ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c20ed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c20ed-126">Request body</span></span>
<span data-ttu-id="c20ed-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c20ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c20ed-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c20ed-128">Response</span></span>
<span data-ttu-id="c20ed-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c20ed-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c20ed-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c20ed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c20ed-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c20ed-131">Request</span></span>
<span data-ttu-id="c20ed-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c20ed-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="c20ed-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c20ed-133">Response</span></span>
<span data-ttu-id="c20ed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c20ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": [
    {
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
  ]
}
```




