---
title: Get deviceManagementExchangeConnector
description: Ler propriedades e relações do objeto deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 49a4b7d84520e3f80dd0035a6e9ec573689518c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866728"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="0d85f-103">Get deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="0d85f-103">Get deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="0d85f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0d85f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d85f-105">Ler propriedades e relações do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="0d85f-105">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d85f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d85f-106">Prerequisites</span></span>
<span data-ttu-id="0d85f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d85f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d85f-109">Permission type</span></span>|<span data-ttu-id="0d85f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d85f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d85f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d85f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d85f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d85f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0d85f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d85f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d85f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d85f-114">Not supported.</span></span>|
|<span data-ttu-id="0d85f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d85f-115">Application</span></span>|<span data-ttu-id="0d85f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d85f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d85f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d85f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d85f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d85f-118">Optional query parameters</span></span>
<span data-ttu-id="0d85f-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d85f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0d85f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d85f-120">Request headers</span></span>
|<span data-ttu-id="0d85f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d85f-121">Header</span></span>|<span data-ttu-id="0d85f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d85f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d85f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d85f-123">Authorization</span></span>|<span data-ttu-id="0d85f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d85f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d85f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d85f-125">Accept</span></span>|<span data-ttu-id="0d85f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d85f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d85f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d85f-127">Request body</span></span>
<span data-ttu-id="0d85f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d85f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d85f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d85f-129">Response</span></span>
<span data-ttu-id="0d85f-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d85f-130">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d85f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d85f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d85f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d85f-132">Request</span></span>
<span data-ttu-id="0d85f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d85f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="0d85f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d85f-134">Response</span></span>
<span data-ttu-id="0d85f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d85f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 580

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
    "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "status": "connectionPending",
    "primarySmtpAddress": "Primary Smtp Address value",
    "serverName": "Server Name value",
    "connectorServerName": "Connector Server Name value",
    "exchangeConnectorType": "hosted",
    "version": "Version value",
    "exchangeAlias": "Exchange Alias value",
    "exchangeOrganization": "Exchange Organization value"
  }
}
```



