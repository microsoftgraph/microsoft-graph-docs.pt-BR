---
title: Listar deviceManagementDomainJoinConnectors
description: Listar propriedades e relações dos objetos deviceManagementDomainJoinConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49f4ed483655eebb9cb93a3e7e0418e241423d7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152744"
---
# <a name="list-devicemanagementdomainjoinconnectors"></a><span data-ttu-id="3bfe3-103">Listar deviceManagementDomainJoinConnectors</span><span class="sxs-lookup"><span data-stu-id="3bfe3-103">List deviceManagementDomainJoinConnectors</span></span>

<span data-ttu-id="3bfe3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bfe3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bfe3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bfe3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bfe3-107">Listar propriedades e relações dos [objetos deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe3-107">List properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bfe3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3bfe3-108">Prerequisites</span></span>
<span data-ttu-id="3bfe3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bfe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bfe3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bfe3-111">Permission type</span></span>|<span data-ttu-id="3bfe3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bfe3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bfe3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bfe3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bfe3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bfe3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bfe3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bfe3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bfe3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-116">Not supported.</span></span>|
|<span data-ttu-id="3bfe3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bfe3-117">Application</span></span>|<span data-ttu-id="3bfe3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bfe3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bfe3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bfe3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="3bfe3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bfe3-120">Request headers</span></span>
|<span data-ttu-id="3bfe3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bfe3-121">Header</span></span>|<span data-ttu-id="3bfe3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3bfe3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bfe3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bfe3-123">Authorization</span></span>|<span data-ttu-id="3bfe3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bfe3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bfe3-125">Accept</span></span>|<span data-ttu-id="3bfe3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bfe3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bfe3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bfe3-127">Request body</span></span>
<span data-ttu-id="3bfe3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bfe3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bfe3-129">Response</span></span>
<span data-ttu-id="3bfe3-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bfe3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bfe3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bfe3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bfe3-132">Request</span></span>
<span data-ttu-id="3bfe3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
```

### <a name="response"></a><span data-ttu-id="3bfe3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bfe3-134">Response</span></span>
<span data-ttu-id="3bfe3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bfe3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
      "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
      "displayName": "Display Name value",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "error",
      "version": "Version value"
    }
  ]
}
```




