---
title: Acessar deviceConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto deviceConfigurationDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a9298424aec45dcd4192e1cdae28484f4276554
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514757"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="ddf11-103">Acessar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="ddf11-103">Get deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="ddf11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddf11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddf11-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddf11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddf11-106">Leia as propriedades e as relações do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ddf11-106">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddf11-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddf11-107">Prerequisites</span></span>
<span data-ttu-id="ddf11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddf11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddf11-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddf11-110">Permission type</span></span>|<span data-ttu-id="ddf11-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddf11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddf11-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddf11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddf11-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddf11-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ddf11-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddf11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddf11-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddf11-115">Not supported.</span></span>|
|<span data-ttu-id="ddf11-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddf11-116">Application</span></span>|<span data-ttu-id="ddf11-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddf11-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddf11-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddf11-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddf11-119">Optional query parameters</span></span>
<span data-ttu-id="ddf11-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf11-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddf11-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf11-121">Request headers</span></span>
|<span data-ttu-id="ddf11-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddf11-122">Header</span></span>|<span data-ttu-id="ddf11-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ddf11-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddf11-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddf11-124">Authorization</span></span>|<span data-ttu-id="ddf11-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddf11-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddf11-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ddf11-126">Accept</span></span>|<span data-ttu-id="ddf11-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ddf11-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddf11-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf11-128">Request body</span></span>
<span data-ttu-id="ddf11-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddf11-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddf11-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf11-130">Response</span></span>
<span data-ttu-id="ddf11-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf11-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddf11-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddf11-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddf11-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf11-133">Request</span></span>
<span data-ttu-id="ddf11-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf11-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="ddf11-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf11-135">Response</span></span>
<span data-ttu-id="ddf11-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddf11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
    "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




