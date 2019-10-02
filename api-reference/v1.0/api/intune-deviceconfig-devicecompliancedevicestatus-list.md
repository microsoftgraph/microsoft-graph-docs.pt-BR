---
title: Listar deviceComplianceDeviceStatuses
description: Listar propriedades e relações dos objetos deviceComplianceDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eefe01be018814f350d469a17b6db3a2a24c8eb9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354298"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="a95db-103">Listar deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a95db-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="a95db-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a95db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a95db-105">Listar propriedades e relações dos objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a95db-105">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a95db-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a95db-106">Prerequisites</span></span>
<span data-ttu-id="a95db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a95db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a95db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a95db-109">Permission type</span></span>|<span data-ttu-id="a95db-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a95db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a95db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a95db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a95db-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a95db-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a95db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a95db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a95db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a95db-114">Not supported.</span></span>|
|<span data-ttu-id="a95db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a95db-115">Application</span></span>|<span data-ttu-id="a95db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a95db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a95db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a95db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a95db-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a95db-118">Request headers</span></span>
|<span data-ttu-id="a95db-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a95db-119">Header</span></span>|<span data-ttu-id="a95db-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a95db-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a95db-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a95db-121">Authorization</span></span>|<span data-ttu-id="a95db-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a95db-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a95db-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a95db-123">Accept</span></span>|<span data-ttu-id="a95db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a95db-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a95db-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a95db-125">Request body</span></span>
<span data-ttu-id="a95db-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a95db-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a95db-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a95db-127">Response</span></span>
<span data-ttu-id="a95db-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a95db-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a95db-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a95db-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a95db-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a95db-130">Request</span></span>
<span data-ttu-id="a95db-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a95db-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="a95db-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a95db-132">Response</span></span>
<span data-ttu-id="a95db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a95db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 544

{
  "value": [
    {
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
  ]
}
```




