---
title: Listar deviceManagementExchangeConnectors
description: Listar propriedades e relações de objeto de deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f5b5488e9a2cd30edb2d8dda45ad0cc3fac1072
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250107"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="91258-103">Listar deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="91258-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="91258-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91258-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91258-105">Listar propriedades e relações de objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="91258-105">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91258-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91258-106">Prerequisites</span></span>
<span data-ttu-id="91258-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="91258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="91258-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91258-109">Permission type</span></span>|<span data-ttu-id="91258-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91258-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91258-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91258-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91258-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="91258-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="91258-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91258-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91258-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91258-114">Not supported.</span></span>|
|<span data-ttu-id="91258-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91258-115">Application</span></span>|<span data-ttu-id="91258-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91258-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91258-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91258-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="91258-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91258-118">Request headers</span></span>
|<span data-ttu-id="91258-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91258-119">Header</span></span>|<span data-ttu-id="91258-120">Valor</span><span class="sxs-lookup"><span data-stu-id="91258-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91258-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="91258-121">Authorization</span></span>|<span data-ttu-id="91258-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91258-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91258-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91258-123">Accept</span></span>|<span data-ttu-id="91258-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91258-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91258-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91258-125">Request body</span></span>
<span data-ttu-id="91258-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91258-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91258-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="91258-127">Response</span></span>
<span data-ttu-id="91258-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91258-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91258-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91258-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="91258-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91258-130">Request</span></span>
<span data-ttu-id="91258-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91258-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="91258-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="91258-132">Response</span></span>
<span data-ttu-id="91258-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91258-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



