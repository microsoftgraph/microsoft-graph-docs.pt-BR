---
title: Obter mobileThreatDefenseConnector
description: Ler propriedades de leitura e relações do objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81391f8d2190567a494fc7137f53e26058c1693a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274800"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="1c3de-103">Obter mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="1c3de-103">Get mobileThreatDefenseConnector</span></span>

<span data-ttu-id="1c3de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c3de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c3de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c3de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c3de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c3de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c3de-107">Ler propriedades de leitura e relações do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="1c3de-107">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c3de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c3de-108">Prerequisites</span></span>
<span data-ttu-id="1c3de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c3de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c3de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c3de-111">Permission type</span></span>|<span data-ttu-id="1c3de-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c3de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c3de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c3de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c3de-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c3de-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1c3de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c3de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c3de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c3de-116">Not supported.</span></span>|
|<span data-ttu-id="1c3de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c3de-117">Application</span></span>|<span data-ttu-id="1c3de-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c3de-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c3de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c3de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c3de-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c3de-120">Optional query parameters</span></span>
<span data-ttu-id="1c3de-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c3de-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c3de-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3de-122">Request headers</span></span>
|<span data-ttu-id="1c3de-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c3de-123">Header</span></span>|<span data-ttu-id="1c3de-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1c3de-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c3de-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c3de-125">Authorization</span></span>|<span data-ttu-id="1c3de-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c3de-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c3de-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c3de-127">Accept</span></span>|<span data-ttu-id="1c3de-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1c3de-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c3de-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3de-129">Request body</span></span>
<span data-ttu-id="1c3de-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c3de-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c3de-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c3de-131">Response</span></span>
<span data-ttu-id="1c3de-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c3de-132">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c3de-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c3de-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c3de-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3de-134">Request</span></span>
<span data-ttu-id="1c3de-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c3de-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="1c3de-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c3de-136">Response</span></span>
<span data-ttu-id="1c3de-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c3de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




