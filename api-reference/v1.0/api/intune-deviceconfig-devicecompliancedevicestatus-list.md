---
title: Listar deviceComplianceDeviceStatuses
description: Listar propriedades e relações dos objetos deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b93c8272d93a851f9ce9228eb0c1a9efabdabffc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760647"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="47eb8-103">Listar deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="47eb8-103">List deviceComplianceDeviceStatuses</span></span>

<span data-ttu-id="47eb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47eb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47eb8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47eb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47eb8-106">Listar propriedades e relações dos objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="47eb8-106">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47eb8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47eb8-107">Prerequisites</span></span>
<span data-ttu-id="47eb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47eb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47eb8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47eb8-110">Permission type</span></span>|<span data-ttu-id="47eb8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47eb8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47eb8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47eb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47eb8-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47eb8-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47eb8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47eb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47eb8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47eb8-115">Not supported.</span></span>|
|<span data-ttu-id="47eb8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47eb8-116">Application</span></span>|<span data-ttu-id="47eb8-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47eb8-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47eb8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47eb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="47eb8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47eb8-119">Request headers</span></span>
|<span data-ttu-id="47eb8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47eb8-120">Header</span></span>|<span data-ttu-id="47eb8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="47eb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47eb8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47eb8-122">Authorization</span></span>|<span data-ttu-id="47eb8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47eb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47eb8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47eb8-124">Accept</span></span>|<span data-ttu-id="47eb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47eb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47eb8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47eb8-126">Request body</span></span>
<span data-ttu-id="47eb8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47eb8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47eb8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="47eb8-128">Response</span></span>
<span data-ttu-id="47eb8-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47eb8-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47eb8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47eb8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="47eb8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47eb8-131">Request</span></span>
<span data-ttu-id="47eb8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47eb8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="47eb8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="47eb8-133">Response</span></span>
<span data-ttu-id="47eb8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47eb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




