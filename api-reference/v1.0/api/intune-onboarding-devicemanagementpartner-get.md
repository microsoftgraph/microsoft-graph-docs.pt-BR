---
title: Acessar deviceManagementPartner
description: Leia as propriedades e as relações do objeto deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51f60eb18aa2d8d454391d737ab279f2ca5230ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35942956"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="742b3-103">Acessar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="742b3-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="742b3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="742b3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="742b3-105">Leia as propriedades e as relações do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="742b3-105">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="742b3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="742b3-106">Prerequisites</span></span>
<span data-ttu-id="742b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="742b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="742b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="742b3-109">Permission type</span></span>|<span data-ttu-id="742b3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="742b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="742b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="742b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="742b3-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="742b3-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="742b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="742b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="742b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="742b3-114">Not supported.</span></span>|
|<span data-ttu-id="742b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="742b3-115">Application</span></span>|<span data-ttu-id="742b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="742b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="742b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="742b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="742b3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="742b3-118">Optional query parameters</span></span>
<span data-ttu-id="742b3-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="742b3-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="742b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="742b3-120">Request headers</span></span>
|<span data-ttu-id="742b3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="742b3-121">Header</span></span>|<span data-ttu-id="742b3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="742b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="742b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="742b3-123">Authorization</span></span>|<span data-ttu-id="742b3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="742b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="742b3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="742b3-125">Accept</span></span>|<span data-ttu-id="742b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="742b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="742b3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="742b3-127">Request body</span></span>
<span data-ttu-id="742b3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="742b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="742b3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="742b3-129">Response</span></span>
<span data-ttu-id="742b3-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="742b3-130">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="742b3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="742b3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="742b3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="742b3-132">Request</span></span>
<span data-ttu-id="742b3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="742b3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="742b3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="742b3-134">Response</span></span>
<span data-ttu-id="742b3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="742b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "value": {
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
}
```



