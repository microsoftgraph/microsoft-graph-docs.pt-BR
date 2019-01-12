---
title: Listar deviceManagementExchangeConnectors
description: Listar propriedades e relações de objeto de deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de6b3ad83765b5e479069698b725a0f7358b1f93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964029"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="e9a90-103">Listar deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="e9a90-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="e9a90-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e9a90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9a90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e9a90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9a90-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e9a90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9a90-107">Listar propriedades e relações de objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="e9a90-107">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9a90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9a90-108">Prerequisites</span></span>
<span data-ttu-id="e9a90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9a90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9a90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9a90-111">Permission type</span></span>|<span data-ttu-id="e9a90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9a90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9a90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9a90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9a90-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9a90-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e9a90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9a90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9a90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9a90-116">Not supported.</span></span>|
|<span data-ttu-id="e9a90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9a90-117">Application</span></span>|<span data-ttu-id="e9a90-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9a90-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9a90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="e9a90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a90-120">Request headers</span></span>
|<span data-ttu-id="e9a90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9a90-121">Header</span></span>|<span data-ttu-id="e9a90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e9a90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9a90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9a90-123">Authorization</span></span>|<span data-ttu-id="e9a90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9a90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9a90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9a90-125">Accept</span></span>|<span data-ttu-id="e9a90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9a90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9a90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a90-127">Request body</span></span>
<span data-ttu-id="e9a90-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9a90-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9a90-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a90-129">Response</span></span>
<span data-ttu-id="e9a90-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a90-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9a90-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9a90-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9a90-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a90-132">Request</span></span>
<span data-ttu-id="e9a90-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9a90-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="e9a90-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a90-134">Response</span></span>
<span data-ttu-id="e9a90-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9a90-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





