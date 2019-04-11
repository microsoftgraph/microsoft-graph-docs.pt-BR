---
title: Get deviceManagementExchangeConnector
description: Ler propriedades e relações do objeto deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eca15c41241032c86e47a36680340a60cf948a3a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779086"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="66046-103">Get deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="66046-103">Get deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="66046-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66046-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66046-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66046-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66046-106">Ler propriedades e relações do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="66046-106">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66046-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66046-107">Prerequisites</span></span>
<span data-ttu-id="66046-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66046-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66046-110">Permission type</span></span>|<span data-ttu-id="66046-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66046-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66046-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66046-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66046-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="66046-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="66046-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66046-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66046-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66046-115">Not supported.</span></span>|
|<span data-ttu-id="66046-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66046-116">Application</span></span>|<span data-ttu-id="66046-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66046-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66046-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66046-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66046-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66046-119">Optional query parameters</span></span>
<span data-ttu-id="66046-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66046-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66046-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66046-121">Request headers</span></span>
|<span data-ttu-id="66046-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66046-122">Header</span></span>|<span data-ttu-id="66046-123">Valor</span><span class="sxs-lookup"><span data-stu-id="66046-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66046-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="66046-124">Authorization</span></span>|<span data-ttu-id="66046-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66046-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66046-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66046-126">Accept</span></span>|<span data-ttu-id="66046-127">application/json</span><span class="sxs-lookup"><span data-stu-id="66046-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66046-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66046-128">Request body</span></span>
<span data-ttu-id="66046-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66046-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66046-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="66046-130">Response</span></span>
<span data-ttu-id="66046-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66046-131">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66046-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66046-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="66046-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66046-133">Request</span></span>
<span data-ttu-id="66046-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66046-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="66046-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="66046-135">Response</span></span>
<span data-ttu-id="66046-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66046-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





