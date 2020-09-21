---
title: Obter mobileThreatDefenseConnector
description: Ler propriedades de leitura e relações do objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e59820a7ad47b896cc1f4f74a44be0519627fb53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969743"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="d3a62-103">Obter mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="d3a62-103">Get mobileThreatDefenseConnector</span></span>

<span data-ttu-id="d3a62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3a62-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3a62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3a62-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3a62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3a62-107">Ler propriedades de leitura e relações do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="d3a62-107">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3a62-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3a62-108">Prerequisites</span></span>
<span data-ttu-id="d3a62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a62-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3a62-111">Permission type</span></span>|<span data-ttu-id="d3a62-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3a62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3a62-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3a62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3a62-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a62-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d3a62-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3a62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3a62-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a62-116">Not supported.</span></span>|
|<span data-ttu-id="d3a62-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3a62-117">Application</span></span>|<span data-ttu-id="d3a62-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a62-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3a62-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3a62-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3a62-120">Optional query parameters</span></span>
<span data-ttu-id="d3a62-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a62-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3a62-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a62-122">Request headers</span></span>
|<span data-ttu-id="d3a62-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3a62-123">Header</span></span>|<span data-ttu-id="d3a62-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d3a62-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3a62-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3a62-125">Authorization</span></span>|<span data-ttu-id="d3a62-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3a62-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3a62-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3a62-127">Accept</span></span>|<span data-ttu-id="d3a62-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d3a62-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a62-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a62-129">Request body</span></span>
<span data-ttu-id="d3a62-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3a62-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3a62-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a62-131">Response</span></span>
<span data-ttu-id="d3a62-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a62-132">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3a62-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3a62-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3a62-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a62-134">Request</span></span>
<span data-ttu-id="d3a62-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3a62-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="d3a62-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a62-136">Response</span></span>
<span data-ttu-id="d3a62-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3a62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






