---
title: Get deviceManagementExchangeConnector
description: Ler propriedades e relações do objeto deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b121e96009b1037cac8d478b4dd9ea1e344ffe9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125846"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="841c8-103">Get deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="841c8-103">Get deviceManagementExchangeConnector</span></span>

<span data-ttu-id="841c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="841c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="841c8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="841c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="841c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="841c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="841c8-107">Ler propriedades e relações do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="841c8-107">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="841c8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="841c8-108">Prerequisites</span></span>
<span data-ttu-id="841c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="841c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="841c8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="841c8-111">Permission type</span></span>|<span data-ttu-id="841c8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="841c8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="841c8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="841c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="841c8-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="841c8-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="841c8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="841c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="841c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="841c8-116">Not supported.</span></span>|
|<span data-ttu-id="841c8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="841c8-117">Application</span></span>|<span data-ttu-id="841c8-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="841c8-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="841c8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="841c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="841c8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="841c8-120">Optional query parameters</span></span>
<span data-ttu-id="841c8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="841c8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="841c8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="841c8-122">Request headers</span></span>
|<span data-ttu-id="841c8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="841c8-123">Header</span></span>|<span data-ttu-id="841c8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="841c8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="841c8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="841c8-125">Authorization</span></span>|<span data-ttu-id="841c8-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="841c8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="841c8-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="841c8-127">Accept</span></span>|<span data-ttu-id="841c8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="841c8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="841c8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="841c8-129">Request body</span></span>
<span data-ttu-id="841c8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="841c8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="841c8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="841c8-131">Response</span></span>
<span data-ttu-id="841c8-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="841c8-132">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="841c8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="841c8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="841c8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="841c8-134">Request</span></span>
<span data-ttu-id="841c8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="841c8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="841c8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="841c8-136">Response</span></span>
<span data-ttu-id="841c8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="841c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




