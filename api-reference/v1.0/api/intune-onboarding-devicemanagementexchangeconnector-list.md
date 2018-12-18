---
title: Listar deviceManagementExchangeConnectors
description: Listar propriedades e relações de objeto de deviceManagementExchangeConnector.
author: tfitzmac
ms.openlocfilehash: 7f3709e22dfc9f545be25500c5f1344ade81d6fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343481"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="6fd19-103">Listar deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="6fd19-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="6fd19-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6fd19-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fd19-105">Listar propriedades e relações de objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="6fd19-105">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fd19-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6fd19-106">Prerequisites</span></span>
<span data-ttu-id="6fd19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fd19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fd19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fd19-109">Permission type</span></span>|<span data-ttu-id="6fd19-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6fd19-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fd19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fd19-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6fd19-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fd19-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6fd19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fd19-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fd19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fd19-114">Not supported.</span></span>|
|<span data-ttu-id="6fd19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fd19-115">Application</span></span>|<span data-ttu-id="6fd19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fd19-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fd19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fd19-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="6fd19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd19-118">Request headers</span></span>
|<span data-ttu-id="6fd19-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fd19-119">Header</span></span>|<span data-ttu-id="6fd19-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6fd19-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fd19-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fd19-121">Authorization</span></span>|<span data-ttu-id="6fd19-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fd19-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fd19-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6fd19-123">Accept</span></span>|<span data-ttu-id="6fd19-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6fd19-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fd19-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd19-125">Request body</span></span>
<span data-ttu-id="6fd19-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fd19-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fd19-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fd19-127">Response</span></span>
<span data-ttu-id="6fd19-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fd19-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fd19-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fd19-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fd19-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd19-130">Request</span></span>
<span data-ttu-id="6fd19-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fd19-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="6fd19-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fd19-132">Response</span></span>
<span data-ttu-id="6fd19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fd19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



