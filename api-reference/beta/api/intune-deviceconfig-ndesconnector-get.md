---
title: Obter ndesConnector
description: Leia as propriedades e as relações do objeto ndesConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9c4dfa2a808b382d6178da7338b861bb6443168
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518220"
---
# <a name="get-ndesconnector"></a><span data-ttu-id="05617-103">Obter ndesConnector</span><span class="sxs-lookup"><span data-stu-id="05617-103">Get ndesConnector</span></span>

> <span data-ttu-id="05617-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05617-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05617-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05617-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05617-106">Leia as propriedades e as relações do objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="05617-106">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05617-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05617-107">Prerequisites</span></span>
<span data-ttu-id="05617-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05617-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05617-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05617-110">Permission type</span></span>|<span data-ttu-id="05617-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05617-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05617-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05617-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05617-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="05617-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="05617-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05617-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05617-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05617-115">Not supported.</span></span>|
|<span data-ttu-id="05617-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05617-116">Application</span></span>|<span data-ttu-id="05617-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05617-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05617-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05617-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05617-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05617-119">Optional query parameters</span></span>
<span data-ttu-id="05617-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05617-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05617-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05617-121">Request headers</span></span>
|<span data-ttu-id="05617-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05617-122">Header</span></span>|<span data-ttu-id="05617-123">Valor</span><span class="sxs-lookup"><span data-stu-id="05617-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05617-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="05617-124">Authorization</span></span>|<span data-ttu-id="05617-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05617-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05617-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05617-126">Accept</span></span>|<span data-ttu-id="05617-127">application/json</span><span class="sxs-lookup"><span data-stu-id="05617-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05617-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05617-128">Request body</span></span>
<span data-ttu-id="05617-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05617-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05617-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="05617-130">Response</span></span>
<span data-ttu-id="05617-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05617-131">If successful, this method returns a `200 OK` response code and [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05617-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05617-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="05617-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05617-133">Request</span></span>
<span data-ttu-id="05617-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05617-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
```

### <a name="response"></a><span data-ttu-id="05617-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="05617-135">Response</span></span>
<span data-ttu-id="05617-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05617-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.ndesConnector",
    "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
    "state": "active",
    "displayName": "Display Name value"
  }
}
```





