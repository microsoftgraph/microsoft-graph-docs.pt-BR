---
title: Listar deviceManagementExchangeConnectors
description: Listar propriedades e relações de objeto de deviceManagementExchangeConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52db3d8f9a87fc85f2f47ab1f017c4f6505da074
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37190760"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="84bf1-103">Listar deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="84bf1-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="84bf1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84bf1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84bf1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84bf1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84bf1-106">Listar propriedades e relações de objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="84bf1-106">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84bf1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84bf1-107">Prerequisites</span></span>
<span data-ttu-id="84bf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84bf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84bf1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84bf1-110">Permission type</span></span>|<span data-ttu-id="84bf1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84bf1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84bf1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84bf1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84bf1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="84bf1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="84bf1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84bf1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84bf1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84bf1-115">Not supported.</span></span>|
|<span data-ttu-id="84bf1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84bf1-116">Application</span></span>|<span data-ttu-id="84bf1-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="84bf1-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84bf1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84bf1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="84bf1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84bf1-119">Request headers</span></span>
|<span data-ttu-id="84bf1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84bf1-120">Header</span></span>|<span data-ttu-id="84bf1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="84bf1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84bf1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="84bf1-122">Authorization</span></span>|<span data-ttu-id="84bf1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84bf1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84bf1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84bf1-124">Accept</span></span>|<span data-ttu-id="84bf1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84bf1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84bf1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84bf1-126">Request body</span></span>
<span data-ttu-id="84bf1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84bf1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84bf1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="84bf1-128">Response</span></span>
<span data-ttu-id="84bf1-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84bf1-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84bf1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84bf1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="84bf1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84bf1-131">Request</span></span>
<span data-ttu-id="84bf1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84bf1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="84bf1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="84bf1-133">Response</span></span>
<span data-ttu-id="84bf1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84bf1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": [
    {
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
  ]
}
```




