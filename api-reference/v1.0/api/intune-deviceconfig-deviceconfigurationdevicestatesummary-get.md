---
title: Obter deviceConfigurationDeviceStateSummary
description: Ler propriedades e relações do objeto deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c1be6f88657b507d2f1375a8b26dcef248db060
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985876"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="3654e-103">Obter deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3654e-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="3654e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3654e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3654e-105">Ler propriedades e relações do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3654e-105">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3654e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3654e-106">Prerequisites</span></span>
<span data-ttu-id="3654e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3654e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3654e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3654e-109">Permission type</span></span>|<span data-ttu-id="3654e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3654e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3654e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3654e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3654e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3654e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3654e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3654e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3654e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3654e-114">Not supported.</span></span>|
|<span data-ttu-id="3654e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3654e-115">Application</span></span>|<span data-ttu-id="3654e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3654e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3654e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3654e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3654e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3654e-118">Optional query parameters</span></span>
<span data-ttu-id="3654e-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3654e-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3654e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3654e-120">Request headers</span></span>
|<span data-ttu-id="3654e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3654e-121">Header</span></span>|<span data-ttu-id="3654e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3654e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3654e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3654e-123">Authorization</span></span>|<span data-ttu-id="3654e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3654e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3654e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3654e-125">Accept</span></span>|<span data-ttu-id="3654e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3654e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3654e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3654e-127">Request body</span></span>
<span data-ttu-id="3654e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3654e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3654e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3654e-129">Response</span></span>
<span data-ttu-id="3654e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3654e-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3654e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3654e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3654e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3654e-132">Request</span></span>
<span data-ttu-id="3654e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3654e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="3654e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3654e-134">Response</span></span>
<span data-ttu-id="3654e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3654e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



