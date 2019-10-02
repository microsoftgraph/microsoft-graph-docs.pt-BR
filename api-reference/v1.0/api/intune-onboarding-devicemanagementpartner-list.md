---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb5ceb82fe0c718774fefdf61c1fac78c954daf7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362362"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="3e92a-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="3e92a-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="3e92a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e92a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e92a-105">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="3e92a-105">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e92a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e92a-106">Prerequisites</span></span>
<span data-ttu-id="3e92a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e92a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e92a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e92a-109">Permission type</span></span>|<span data-ttu-id="3e92a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e92a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e92a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e92a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e92a-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e92a-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3e92a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e92a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e92a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e92a-114">Not supported.</span></span>|
|<span data-ttu-id="3e92a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e92a-115">Application</span></span>|<span data-ttu-id="3e92a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e92a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e92a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e92a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="3e92a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e92a-118">Request headers</span></span>
|<span data-ttu-id="3e92a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e92a-119">Header</span></span>|<span data-ttu-id="3e92a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3e92a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e92a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e92a-121">Authorization</span></span>|<span data-ttu-id="3e92a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e92a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e92a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e92a-123">Accept</span></span>|<span data-ttu-id="3e92a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3e92a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e92a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e92a-125">Request body</span></span>
<span data-ttu-id="3e92a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e92a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e92a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e92a-127">Response</span></span>
<span data-ttu-id="3e92a-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e92a-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e92a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e92a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e92a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e92a-130">Request</span></span>
<span data-ttu-id="3e92a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e92a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="3e92a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e92a-132">Response</span></span>
<span data-ttu-id="3e92a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e92a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




