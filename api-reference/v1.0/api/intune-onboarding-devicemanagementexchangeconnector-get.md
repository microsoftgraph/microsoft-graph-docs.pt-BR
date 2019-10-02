---
title: Get deviceManagementExchangeConnector
description: Ler propriedades e relações do objeto deviceManagementExchangeConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b74e3148f11f7dcf25197cfd222cc7cfcd1d19b3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362474"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="92958-103">Get deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="92958-103">Get deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="92958-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92958-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92958-105">Ler propriedades e relações do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="92958-105">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92958-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92958-106">Prerequisites</span></span>
<span data-ttu-id="92958-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92958-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92958-109">Permission type</span></span>|<span data-ttu-id="92958-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92958-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92958-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92958-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92958-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="92958-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="92958-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92958-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92958-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92958-114">Not supported.</span></span>|
|<span data-ttu-id="92958-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92958-115">Application</span></span>|<span data-ttu-id="92958-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92958-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92958-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92958-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92958-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92958-118">Optional query parameters</span></span>
<span data-ttu-id="92958-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92958-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92958-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92958-120">Request headers</span></span>
|<span data-ttu-id="92958-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92958-121">Header</span></span>|<span data-ttu-id="92958-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92958-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92958-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92958-123">Authorization</span></span>|<span data-ttu-id="92958-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92958-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92958-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92958-125">Accept</span></span>|<span data-ttu-id="92958-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92958-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92958-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92958-127">Request body</span></span>
<span data-ttu-id="92958-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92958-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92958-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="92958-129">Response</span></span>
<span data-ttu-id="92958-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92958-130">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92958-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92958-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="92958-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92958-132">Request</span></span>
<span data-ttu-id="92958-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92958-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="92958-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="92958-134">Response</span></span>
<span data-ttu-id="92958-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92958-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




