---
title: Obter deviceConfigurationDeviceStateSummary
description: Ler propriedades e relações do objeto deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bca4bc924fd0cebdbbc003ff64f79cbdb919f9da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770337"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="37683-103">Obter deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="37683-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="37683-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37683-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37683-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37683-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37683-106">Ler propriedades e relações do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="37683-106">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37683-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37683-107">Prerequisites</span></span>
<span data-ttu-id="37683-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37683-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37683-110">Permission type</span></span>|<span data-ttu-id="37683-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37683-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37683-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37683-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37683-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37683-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="37683-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37683-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37683-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37683-115">Not supported.</span></span>|
|<span data-ttu-id="37683-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37683-116">Application</span></span>|<span data-ttu-id="37683-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37683-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37683-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37683-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37683-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37683-119">Optional query parameters</span></span>
<span data-ttu-id="37683-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37683-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37683-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37683-121">Request headers</span></span>
|<span data-ttu-id="37683-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37683-122">Header</span></span>|<span data-ttu-id="37683-123">Valor</span><span class="sxs-lookup"><span data-stu-id="37683-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37683-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="37683-124">Authorization</span></span>|<span data-ttu-id="37683-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37683-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37683-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37683-126">Accept</span></span>|<span data-ttu-id="37683-127">application/json</span><span class="sxs-lookup"><span data-stu-id="37683-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37683-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37683-128">Request body</span></span>
<span data-ttu-id="37683-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37683-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37683-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="37683-130">Response</span></span>
<span data-ttu-id="37683-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37683-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37683-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37683-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="37683-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37683-133">Request</span></span>
<span data-ttu-id="37683-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37683-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="37683-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="37683-135">Response</span></span>
<span data-ttu-id="37683-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37683-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
    "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```





