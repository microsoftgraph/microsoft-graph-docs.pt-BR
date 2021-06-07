---
title: Acessar deviceManagementPartner
description: Leia as propriedades e as relações do objeto deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b261567a1edeb26310ef696ab0f0a7e24a8b6d4a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758014"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="358dd-103">Acessar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="358dd-103">Get deviceManagementPartner</span></span>

<span data-ttu-id="358dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="358dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="358dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="358dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="358dd-106">Leia as propriedades e as relações do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="358dd-106">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="358dd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="358dd-107">Prerequisites</span></span>
<span data-ttu-id="358dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="358dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="358dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="358dd-110">Permission type</span></span>|<span data-ttu-id="358dd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="358dd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="358dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="358dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="358dd-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="358dd-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="358dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="358dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="358dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="358dd-115">Not supported.</span></span>|
|<span data-ttu-id="358dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="358dd-116">Application</span></span>|<span data-ttu-id="358dd-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="358dd-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="358dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="358dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="358dd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="358dd-119">Optional query parameters</span></span>
<span data-ttu-id="358dd-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="358dd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="358dd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="358dd-121">Request headers</span></span>
|<span data-ttu-id="358dd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="358dd-122">Header</span></span>|<span data-ttu-id="358dd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="358dd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="358dd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="358dd-124">Authorization</span></span>|<span data-ttu-id="358dd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="358dd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="358dd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="358dd-126">Accept</span></span>|<span data-ttu-id="358dd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="358dd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="358dd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="358dd-128">Request body</span></span>
<span data-ttu-id="358dd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="358dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="358dd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="358dd-130">Response</span></span>
<span data-ttu-id="358dd-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="358dd-131">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="358dd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="358dd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="358dd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="358dd-133">Request</span></span>
<span data-ttu-id="358dd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="358dd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="358dd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="358dd-135">Response</span></span>
<span data-ttu-id="358dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="358dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




