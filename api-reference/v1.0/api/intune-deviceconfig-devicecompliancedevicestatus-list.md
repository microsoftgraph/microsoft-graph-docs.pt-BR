---
title: Listar deviceComplianceDeviceStatuses
description: Listar propriedades e relações dos objetos deviceComplianceDeviceStatus.
ms.openlocfilehash: 318852070070ec2d067ece30f7deaadb8b5aaa4b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004915"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="91d0e-103">Listar deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="91d0e-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="91d0e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="91d0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91d0e-105">Listar propriedades e relações dos objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="91d0e-105">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91d0e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91d0e-106">Prerequisites</span></span>
<span data-ttu-id="91d0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91d0e-109">Permission type</span></span>|<span data-ttu-id="91d0e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91d0e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91d0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91d0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91d0e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="91d0e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="91d0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91d0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91d0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91d0e-114">Not supported.</span></span>|
|<span data-ttu-id="91d0e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91d0e-115">Application</span></span>|<span data-ttu-id="91d0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91d0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91d0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91d0e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="91d0e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91d0e-118">Request headers</span></span>
|<span data-ttu-id="91d0e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91d0e-119">Header</span></span>|<span data-ttu-id="91d0e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="91d0e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91d0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="91d0e-121">Authorization</span></span>|<span data-ttu-id="91d0e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91d0e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91d0e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="91d0e-123">Accept</span></span>|<span data-ttu-id="91d0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91d0e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91d0e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91d0e-125">Request body</span></span>
<span data-ttu-id="91d0e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91d0e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91d0e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="91d0e-127">Response</span></span>
<span data-ttu-id="91d0e-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91d0e-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d0e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91d0e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="91d0e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91d0e-130">Request</span></span>
<span data-ttu-id="91d0e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91d0e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="91d0e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="91d0e-132">Response</span></span>
<span data-ttu-id="91d0e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91d0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



