---
title: Listar deviceManagementExchangeConnectors
description: Listar propriedades e relações de objeto de deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db069b32025718f4fdaee71291322b5cd0218fe4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972088"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="b1296-103">Listar deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="b1296-103">List deviceManagementExchangeConnectors</span></span>

<span data-ttu-id="b1296-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1296-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1296-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1296-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1296-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1296-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1296-107">Listar propriedades e relações de objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b1296-107">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1296-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1296-108">Prerequisites</span></span>
<span data-ttu-id="b1296-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1296-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1296-111">Permission type</span></span>|<span data-ttu-id="b1296-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1296-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1296-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1296-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1296-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1296-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b1296-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1296-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1296-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1296-116">Not supported.</span></span>|
|<span data-ttu-id="b1296-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1296-117">Application</span></span>|<span data-ttu-id="b1296-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1296-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1296-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1296-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="b1296-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1296-120">Request headers</span></span>
|<span data-ttu-id="b1296-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1296-121">Header</span></span>|<span data-ttu-id="b1296-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1296-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1296-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1296-123">Authorization</span></span>|<span data-ttu-id="b1296-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1296-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1296-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1296-125">Accept</span></span>|<span data-ttu-id="b1296-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1296-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1296-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1296-127">Request body</span></span>
<span data-ttu-id="b1296-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1296-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1296-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1296-129">Response</span></span>
<span data-ttu-id="b1296-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1296-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1296-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1296-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1296-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1296-132">Request</span></span>
<span data-ttu-id="b1296-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1296-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="b1296-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1296-134">Response</span></span>
<span data-ttu-id="b1296-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1296-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






