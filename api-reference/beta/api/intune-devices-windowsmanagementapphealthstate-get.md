---
title: Obter windowsManagementAppHealthState
description: Leia as propriedades e os relacionamentos do objeto windowsManagementAppHealthState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 43030b06ea2913132e43086bd8eec9af3a616262
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828543"
---
# <a name="get-windowsmanagementapphealthstate"></a><span data-ttu-id="78832-103">Obter windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="78832-103">Get windowsManagementAppHealthState</span></span>

> <span data-ttu-id="78832-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78832-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78832-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78832-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78832-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="78832-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78832-107">Leia as propriedades e os relacionamentos do objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="78832-107">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78832-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78832-108">Prerequisites</span></span>
<span data-ttu-id="78832-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78832-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78832-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78832-111">Permission type</span></span>|<span data-ttu-id="78832-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78832-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78832-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78832-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78832-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="78832-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="78832-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78832-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78832-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78832-116">Not supported.</span></span>|
|<span data-ttu-id="78832-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78832-117">Application</span></span>|<span data-ttu-id="78832-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78832-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78832-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78832-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78832-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78832-120">Optional query parameters</span></span>
<span data-ttu-id="78832-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78832-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="78832-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78832-122">Request headers</span></span>
|<span data-ttu-id="78832-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78832-123">Header</span></span>|<span data-ttu-id="78832-124">Valor</span><span class="sxs-lookup"><span data-stu-id="78832-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78832-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="78832-125">Authorization</span></span>|<span data-ttu-id="78832-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78832-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78832-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78832-127">Accept</span></span>|<span data-ttu-id="78832-128">application/json</span><span class="sxs-lookup"><span data-stu-id="78832-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78832-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78832-129">Request body</span></span>
<span data-ttu-id="78832-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78832-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78832-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="78832-131">Response</span></span>
<span data-ttu-id="78832-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78832-132">If successful, this method returns a `200 OK` response code and [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78832-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78832-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="78832-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78832-134">Request</span></span>
<span data-ttu-id="78832-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78832-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

### <a name="response"></a><span data-ttu-id="78832-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="78832-136">Response</span></span>
<span data-ttu-id="78832-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78832-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
    "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
    "healthState": "healthy",
    "installedVersion": "Installed Version value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
    "deviceName": "Device Name value",
    "deviceOSVersion": "Device OSVersion value"
  }
}
```





