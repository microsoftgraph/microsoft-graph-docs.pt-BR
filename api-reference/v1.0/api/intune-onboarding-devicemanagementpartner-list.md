---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 465ac4b2718fcc8e689c816dbb1cd4d8efa8654c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512514"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="8f417-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="8f417-103">List deviceManagementPartners</span></span>

<span data-ttu-id="8f417-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f417-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f417-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f417-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f417-106">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8f417-106">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f417-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f417-107">Prerequisites</span></span>
<span data-ttu-id="8f417-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f417-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f417-110">Permission type</span></span>|<span data-ttu-id="8f417-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f417-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f417-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f417-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f417-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f417-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8f417-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f417-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f417-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f417-115">Not supported.</span></span>|
|<span data-ttu-id="8f417-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f417-116">Application</span></span>|<span data-ttu-id="8f417-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f417-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f417-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f417-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8f417-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f417-119">Request headers</span></span>
|<span data-ttu-id="8f417-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f417-120">Header</span></span>|<span data-ttu-id="8f417-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8f417-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f417-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f417-122">Authorization</span></span>|<span data-ttu-id="8f417-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f417-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f417-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f417-124">Accept</span></span>|<span data-ttu-id="8f417-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f417-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f417-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f417-126">Request body</span></span>
<span data-ttu-id="8f417-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f417-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f417-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f417-128">Response</span></span>
<span data-ttu-id="8f417-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f417-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f417-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f417-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f417-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f417-131">Request</span></span>
<span data-ttu-id="8f417-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f417-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="8f417-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f417-133">Response</span></span>
<span data-ttu-id="8f417-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f417-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




