---
title: Obter mobileThreatDefenseConnector
description: Propriedades de leitura e relações do objeto mobileThreatDefenseConnector.
ms.openlocfilehash: 7b63cdd7fc9476ad36f8bf249e0b5a358414b9fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039193"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="d47dd-103">Obter mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="d47dd-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="d47dd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d47dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d47dd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d47dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d47dd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d47dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d47dd-107">Ler propriedades de leitura e relações do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="d47dd-107">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d47dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d47dd-108">Prerequisites</span></span>
<span data-ttu-id="d47dd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d47dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d47dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d47dd-111">Permission type</span></span>|<span data-ttu-id="d47dd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d47dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d47dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d47dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d47dd-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47dd-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d47dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d47dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d47dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d47dd-116">Not supported.</span></span>|
|<span data-ttu-id="d47dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d47dd-117">Application</span></span>|<span data-ttu-id="d47dd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d47dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d47dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d47dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d47dd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d47dd-120">Optional query parameters</span></span>
<span data-ttu-id="d47dd-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d47dd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d47dd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d47dd-122">Request headers</span></span>
|<span data-ttu-id="d47dd-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d47dd-123">Header</span></span>|<span data-ttu-id="d47dd-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d47dd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d47dd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d47dd-125">Authorization</span></span>|<span data-ttu-id="d47dd-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d47dd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d47dd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d47dd-127">Accept</span></span>|<span data-ttu-id="d47dd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d47dd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d47dd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d47dd-129">Request body</span></span>
<span data-ttu-id="d47dd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d47dd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d47dd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d47dd-131">Response</span></span>
<span data-ttu-id="d47dd-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d47dd-132">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d47dd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d47dd-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d47dd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d47dd-134">Request</span></span>
<span data-ttu-id="d47dd-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d47dd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="d47dd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d47dd-136">Response</span></span>
<span data-ttu-id="d47dd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d47dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





