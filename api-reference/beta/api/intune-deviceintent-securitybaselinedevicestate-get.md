---
title: Obter securityBaselineDeviceState
description: Leia as propriedades e as relações do objeto securityBaselineDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 372aeefd9e658b2f4df2b201adf15373167ee428
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959527"
---
# <a name="get-securitybaselinedevicestate"></a><span data-ttu-id="45e52-103">Obter securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="45e52-103">Get securityBaselineDeviceState</span></span>

> <span data-ttu-id="45e52-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45e52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45e52-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45e52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45e52-106">Leia as propriedades e as relações do objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="45e52-106">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45e52-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45e52-107">Prerequisites</span></span>
<span data-ttu-id="45e52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45e52-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45e52-110">Permission type</span></span>|<span data-ttu-id="45e52-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45e52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45e52-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45e52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45e52-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45e52-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45e52-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45e52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45e52-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45e52-115">Not supported.</span></span>|
|<span data-ttu-id="45e52-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45e52-116">Application</span></span>|<span data-ttu-id="45e52-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45e52-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45e52-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45e52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45e52-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45e52-119">Optional query parameters</span></span>
<span data-ttu-id="45e52-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45e52-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45e52-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45e52-121">Request headers</span></span>
|<span data-ttu-id="45e52-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45e52-122">Header</span></span>|<span data-ttu-id="45e52-123">Valor</span><span class="sxs-lookup"><span data-stu-id="45e52-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45e52-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="45e52-124">Authorization</span></span>|<span data-ttu-id="45e52-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45e52-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45e52-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45e52-126">Accept</span></span>|<span data-ttu-id="45e52-127">application/json</span><span class="sxs-lookup"><span data-stu-id="45e52-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45e52-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45e52-128">Request body</span></span>
<span data-ttu-id="45e52-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45e52-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45e52-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="45e52-130">Response</span></span>
<span data-ttu-id="45e52-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45e52-131">If successful, this method returns a `200 OK` response code and [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45e52-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45e52-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="45e52-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45e52-133">Request</span></span>
<span data-ttu-id="45e52-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45e52-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="45e52-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="45e52-135">Response</span></span>
<span data-ttu-id="45e52-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45e52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
    "id": "182749bf-49bf-1827-bf49-2718bf492718",
    "managedDeviceId": "Managed Device Id value",
    "deviceDisplayName": "Device Display Name value",
    "userPrincipalName": "User Principal Name value",
    "state": "secure",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```





