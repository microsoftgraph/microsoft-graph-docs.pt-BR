---
title: Listar ndesConnectors
description: Listar Propriedades e relações dos objetos ndesConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac49bbf813fe31479d8c14fb8676aee9b7caee57
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442031"
---
# <a name="list-ndesconnectors"></a><span data-ttu-id="7922f-103">Listar ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="7922f-103">List ndesConnectors</span></span>

<span data-ttu-id="7922f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7922f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7922f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7922f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7922f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7922f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7922f-107">Listar Propriedades e relações dos objetos [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="7922f-107">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7922f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7922f-108">Prerequisites</span></span>
<span data-ttu-id="7922f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7922f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7922f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7922f-111">Permission type</span></span>|<span data-ttu-id="7922f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7922f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7922f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7922f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7922f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7922f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7922f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7922f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7922f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7922f-116">Not supported.</span></span>|
|<span data-ttu-id="7922f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7922f-117">Application</span></span>|<span data-ttu-id="7922f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7922f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7922f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7922f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="7922f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7922f-120">Request headers</span></span>
|<span data-ttu-id="7922f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7922f-121">Header</span></span>|<span data-ttu-id="7922f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7922f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7922f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7922f-123">Authorization</span></span>|<span data-ttu-id="7922f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7922f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7922f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7922f-125">Accept</span></span>|<span data-ttu-id="7922f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7922f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7922f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7922f-127">Request body</span></span>
<span data-ttu-id="7922f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7922f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7922f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7922f-129">Response</span></span>
<span data-ttu-id="7922f-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7922f-130">If successful, this method returns a `200 OK` response code and a collection of [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7922f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7922f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7922f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7922f-132">Request</span></span>
<span data-ttu-id="7922f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7922f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
```

### <a name="response"></a><span data-ttu-id="7922f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7922f-134">Response</span></span>
<span data-ttu-id="7922f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7922f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ndesConnector",
      "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "active",
      "displayName": "Display Name value"
    }
  ]
}
```





