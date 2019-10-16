---
title: Obter mobileThreatDefenseConnector
description: Ler propriedades de leitura e relações do objeto mobileThreatDefenseConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c8c206391742c438d262c3247b1a748f32e8b67
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536550"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="28905-103">Obter mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="28905-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="28905-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28905-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28905-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28905-106">Ler propriedades de leitura e relações do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="28905-106">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28905-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28905-107">Prerequisites</span></span>
<span data-ttu-id="28905-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28905-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28905-110">Permission type</span></span>|<span data-ttu-id="28905-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28905-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28905-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28905-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28905-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="28905-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="28905-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28905-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28905-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28905-115">Not supported.</span></span>|
|<span data-ttu-id="28905-116">Application</span><span class="sxs-lookup"><span data-stu-id="28905-116">Application</span></span>|<span data-ttu-id="28905-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="28905-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28905-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28905-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28905-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28905-119">Optional query parameters</span></span>
<span data-ttu-id="28905-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28905-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28905-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28905-121">Request headers</span></span>
|<span data-ttu-id="28905-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28905-122">Header</span></span>|<span data-ttu-id="28905-123">Valor</span><span class="sxs-lookup"><span data-stu-id="28905-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28905-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="28905-124">Authorization</span></span>|<span data-ttu-id="28905-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28905-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28905-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28905-126">Accept</span></span>|<span data-ttu-id="28905-127">application/json</span><span class="sxs-lookup"><span data-stu-id="28905-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28905-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28905-128">Request body</span></span>
<span data-ttu-id="28905-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28905-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28905-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="28905-130">Response</span></span>
<span data-ttu-id="28905-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28905-131">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28905-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28905-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="28905-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28905-133">Request</span></span>
<span data-ttu-id="28905-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28905-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="28905-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="28905-135">Response</span></span>
<span data-ttu-id="28905-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 828

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidMobileApplicationManagementEnabled": true,
    "iosMobileApplicationManagementEnabled": true,
    "androidEnabled": true,
    "iosEnabled": true,
    "windowsEnabled": true,
    "macEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "windowsDeviceBlockedOnMissingPartnerData": true,
    "macDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6,
    "allowPartnerToCollectIOSApplicationMetadata": true
  }
}
```






