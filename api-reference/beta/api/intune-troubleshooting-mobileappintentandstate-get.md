---
title: Obter mobileAppIntentAndState
description: Leia as propriedades e as relações do objeto mobileAppIntentAndState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26b0db271955c26ffdd58b5d4449d7f874cc787b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195367"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="63198-103">Obter mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="63198-103">Get mobileAppIntentAndState</span></span>

> <span data-ttu-id="63198-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63198-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63198-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63198-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63198-106">Leia as propriedades e as relações do objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="63198-106">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63198-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63198-107">Prerequisites</span></span>
<span data-ttu-id="63198-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63198-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63198-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63198-110">Permission type</span></span>|<span data-ttu-id="63198-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63198-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63198-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63198-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63198-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="63198-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="63198-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63198-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63198-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63198-115">Not supported.</span></span>|
|<span data-ttu-id="63198-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63198-116">Application</span></span>|<span data-ttu-id="63198-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="63198-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63198-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63198-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63198-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="63198-119">Optional query parameters</span></span>
<span data-ttu-id="63198-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="63198-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63198-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63198-121">Request headers</span></span>
|<span data-ttu-id="63198-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63198-122">Header</span></span>|<span data-ttu-id="63198-123">Valor</span><span class="sxs-lookup"><span data-stu-id="63198-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63198-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="63198-124">Authorization</span></span>|<span data-ttu-id="63198-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63198-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63198-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63198-126">Accept</span></span>|<span data-ttu-id="63198-127">application/json</span><span class="sxs-lookup"><span data-stu-id="63198-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63198-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63198-128">Request body</span></span>
<span data-ttu-id="63198-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63198-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63198-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="63198-130">Response</span></span>
<span data-ttu-id="63198-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63198-131">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63198-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63198-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="63198-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63198-133">Request</span></span>
<span data-ttu-id="63198-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63198-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="63198-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="63198-135">Response</span></span>
<span data-ttu-id="63198-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63198-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 943

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
    "id": "45a775d6-75d6-45a7-d675-a745d675a745",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "userId": "User Id value",
    "mobileAppList": [
      {
        "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
        "applicationId": "Application Id value",
        "displayName": "Display Name value",
        "mobileAppIntent": "notAvailable",
        "displayVersion": "Display Version value",
        "installState": "failed",
        "supportedDeviceTypes": [
          {
            "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
            "type": "windowsRT",
            "minimumOperatingSystemVersion": "Minimum Operating System Version value",
            "maximumOperatingSystemVersion": "Maximum Operating System Version value"
          }
        ]
      }
    ]
  }
}
```




