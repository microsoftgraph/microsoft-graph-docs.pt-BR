---
title: Get deviceComplianceDeviceStatus
description: Ler propriedades e relações do objeto deviceComplianceDeviceStatus.
ms.openlocfilehash: 0f4b2ad05807ac1a1c5f134bad9cfaa24046c510
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040141"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="f2a03-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f2a03-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="f2a03-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2a03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2a03-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2a03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2a03-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2a03-107">Ler propriedades e relações do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f2a03-107">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2a03-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2a03-108">Prerequisites</span></span>
<span data-ttu-id="f2a03-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2a03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2a03-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2a03-111">Permission type</span></span>|<span data-ttu-id="f2a03-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2a03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2a03-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2a03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2a03-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2a03-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2a03-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2a03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2a03-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2a03-116">Not supported.</span></span>|
|<span data-ttu-id="f2a03-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2a03-117">Application</span></span>|<span data-ttu-id="f2a03-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2a03-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2a03-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2a03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2a03-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2a03-120">Optional query parameters</span></span>
<span data-ttu-id="f2a03-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2a03-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f2a03-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a03-122">Request headers</span></span>
|<span data-ttu-id="f2a03-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2a03-123">Header</span></span>|<span data-ttu-id="f2a03-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f2a03-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2a03-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2a03-125">Authorization</span></span>|<span data-ttu-id="f2a03-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2a03-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2a03-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f2a03-127">Accept</span></span>|<span data-ttu-id="f2a03-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a03-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a03-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a03-129">Request body</span></span>
<span data-ttu-id="f2a03-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2a03-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2a03-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a03-131">Response</span></span>
<span data-ttu-id="f2a03-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2a03-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a03-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2a03-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2a03-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a03-134">Request</span></span>
<span data-ttu-id="f2a03-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2a03-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="f2a03-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a03-136">Response</span></span>
<span data-ttu-id="f2a03-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2a03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





