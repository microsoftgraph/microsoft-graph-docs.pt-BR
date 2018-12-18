---
title: Acessar deviceConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto deviceConfigurationDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 8bafdda535bd6737454370bd640efc3c9f7869b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339267"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="4ab81-103">Acessar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4ab81-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="4ab81-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ab81-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ab81-105">Leia as propriedades e as relações do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4ab81-105">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ab81-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ab81-106">Prerequisites</span></span>
<span data-ttu-id="4ab81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ab81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab81-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ab81-109">Permission type</span></span>|<span data-ttu-id="4ab81-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ab81-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ab81-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ab81-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ab81-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ab81-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ab81-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ab81-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ab81-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ab81-114">Not supported.</span></span>|
|<span data-ttu-id="4ab81-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ab81-115">Application</span></span>|<span data-ttu-id="4ab81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ab81-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ab81-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ab81-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ab81-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ab81-118">Optional query parameters</span></span>
<span data-ttu-id="4ab81-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ab81-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ab81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab81-120">Request headers</span></span>
|<span data-ttu-id="4ab81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ab81-121">Header</span></span>|<span data-ttu-id="4ab81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ab81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ab81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ab81-123">Authorization</span></span>|<span data-ttu-id="4ab81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ab81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ab81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ab81-125">Accept</span></span>|<span data-ttu-id="4ab81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ab81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ab81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab81-127">Request body</span></span>
<span data-ttu-id="4ab81-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ab81-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab81-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ab81-129">Response</span></span>
<span data-ttu-id="4ab81-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ab81-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ab81-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ab81-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ab81-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab81-132">Request</span></span>
<span data-ttu-id="4ab81-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ab81-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="4ab81-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ab81-134">Response</span></span>
<span data-ttu-id="4ab81-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ab81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



