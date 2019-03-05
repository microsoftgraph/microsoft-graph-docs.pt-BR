---
title: Obter mobileThreatDefenseConnector
description: Propriedades de leitura e relações do objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8668ba21a4135cf15edf5d6b211859d072060e9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148689"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="71002-103">Obter mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="71002-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="71002-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71002-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71002-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71002-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71002-106">Ler propriedades de leitura e relações do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="71002-106">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71002-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71002-107">Prerequisites</span></span>
<span data-ttu-id="71002-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71002-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71002-110">Permission type</span></span>|<span data-ttu-id="71002-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71002-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71002-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71002-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71002-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="71002-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="71002-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71002-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71002-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71002-115">Not supported.</span></span>|
|<span data-ttu-id="71002-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71002-116">Application</span></span>|<span data-ttu-id="71002-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71002-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71002-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71002-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71002-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71002-119">Optional query parameters</span></span>
<span data-ttu-id="71002-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71002-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71002-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71002-121">Request headers</span></span>
|<span data-ttu-id="71002-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71002-122">Header</span></span>|<span data-ttu-id="71002-123">Valor</span><span class="sxs-lookup"><span data-stu-id="71002-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71002-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="71002-124">Authorization</span></span>|<span data-ttu-id="71002-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71002-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71002-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71002-126">Accept</span></span>|<span data-ttu-id="71002-127">application/json</span><span class="sxs-lookup"><span data-stu-id="71002-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71002-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71002-128">Request body</span></span>
<span data-ttu-id="71002-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71002-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71002-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="71002-130">Response</span></span>
<span data-ttu-id="71002-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71002-131">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71002-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71002-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="71002-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71002-133">Request</span></span>
<span data-ttu-id="71002-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71002-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="71002-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="71002-135">Response</span></span>
<span data-ttu-id="71002-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71002-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 720

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
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




