---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
ms.openlocfilehash: c308dc378fdcd0257b72b4a5948635ec0c1fa257
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004242"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="e4923-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="e4923-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="e4923-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e4923-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4923-105">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e4923-105">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4923-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4923-106">Prerequisites</span></span>
<span data-ttu-id="e4923-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4923-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4923-109">Permission type</span></span>|<span data-ttu-id="e4923-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4923-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4923-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4923-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4923-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4923-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e4923-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4923-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4923-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4923-114">Not supported.</span></span>|
|<span data-ttu-id="e4923-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4923-115">Application</span></span>|<span data-ttu-id="e4923-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4923-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4923-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4923-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e4923-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4923-118">Request headers</span></span>
|<span data-ttu-id="e4923-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4923-119">Header</span></span>|<span data-ttu-id="e4923-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e4923-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4923-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4923-121">Authorization</span></span>|<span data-ttu-id="e4923-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4923-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4923-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e4923-123">Accept</span></span>|<span data-ttu-id="e4923-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e4923-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4923-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4923-125">Request body</span></span>
<span data-ttu-id="e4923-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4923-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4923-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4923-127">Response</span></span>
<span data-ttu-id="e4923-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4923-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4923-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4923-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4923-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4923-130">Request</span></span>
<span data-ttu-id="e4923-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4923-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="e4923-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4923-132">Response</span></span>
<span data-ttu-id="e4923-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4923-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```



