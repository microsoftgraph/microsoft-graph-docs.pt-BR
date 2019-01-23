---
title: Get deviceManagementExchangeConnector
description: Ler propriedades e relações do objeto deviceManagementExchangeConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 14b487f813ed8c52842d8e5a2f7665c88ffacacf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416423"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="0a310-103">Get deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="0a310-103">Get deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="0a310-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a310-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0a310-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a310-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a310-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0a310-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a310-107">Ler propriedades e relações do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="0a310-107">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a310-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a310-108">Prerequisites</span></span>
<span data-ttu-id="0a310-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a310-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0a310-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a310-111">Permission type</span></span>|<span data-ttu-id="0a310-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a310-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a310-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a310-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a310-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a310-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0a310-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a310-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a310-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a310-116">Not supported.</span></span>|
|<span data-ttu-id="0a310-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a310-117">Application</span></span>|<span data-ttu-id="0a310-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a310-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a310-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a310-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a310-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a310-120">Optional query parameters</span></span>
<span data-ttu-id="0a310-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a310-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a310-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a310-122">Request headers</span></span>
|<span data-ttu-id="0a310-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a310-123">Header</span></span>|<span data-ttu-id="0a310-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0a310-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a310-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a310-125">Authorization</span></span>|<span data-ttu-id="0a310-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a310-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a310-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a310-127">Accept</span></span>|<span data-ttu-id="0a310-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0a310-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a310-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a310-129">Request body</span></span>
<span data-ttu-id="0a310-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a310-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a310-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a310-131">Response</span></span>
<span data-ttu-id="0a310-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a310-132">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a310-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a310-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a310-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a310-134">Request</span></span>
<span data-ttu-id="0a310-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a310-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="0a310-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a310-136">Response</span></span>
<span data-ttu-id="0a310-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a310-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




