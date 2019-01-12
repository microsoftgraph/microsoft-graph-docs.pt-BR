---
title: Listar deviceComplianceDeviceStatuses
description: Listar propriedades e relações dos objetos deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd7472893cd5dbb5abad6f892506e1778f534b29
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940320"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="66e14-103">Listar deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="66e14-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="66e14-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66e14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66e14-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66e14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66e14-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="66e14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66e14-107">Listar propriedades e relações dos objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="66e14-107">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66e14-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66e14-108">Prerequisites</span></span>
<span data-ttu-id="66e14-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66e14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66e14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66e14-111">Permission type</span></span>|<span data-ttu-id="66e14-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66e14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66e14-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66e14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66e14-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="66e14-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="66e14-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66e14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66e14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66e14-116">Not supported.</span></span>|
|<span data-ttu-id="66e14-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66e14-117">Application</span></span>|<span data-ttu-id="66e14-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66e14-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66e14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66e14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="66e14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66e14-120">Request headers</span></span>
|<span data-ttu-id="66e14-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66e14-121">Header</span></span>|<span data-ttu-id="66e14-122">Valor</span><span class="sxs-lookup"><span data-stu-id="66e14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66e14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="66e14-123">Authorization</span></span>|<span data-ttu-id="66e14-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66e14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66e14-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66e14-125">Accept</span></span>|<span data-ttu-id="66e14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66e14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e14-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66e14-127">Request body</span></span>
<span data-ttu-id="66e14-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66e14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66e14-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e14-129">Response</span></span>
<span data-ttu-id="66e14-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66e14-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66e14-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66e14-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="66e14-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e14-132">Request</span></span>
<span data-ttu-id="66e14-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66e14-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="66e14-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e14-134">Response</span></span>
<span data-ttu-id="66e14-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66e14-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





