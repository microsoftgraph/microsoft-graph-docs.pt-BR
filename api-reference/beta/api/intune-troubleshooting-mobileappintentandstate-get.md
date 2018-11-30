---
title: Obter mobileAppIntentAndState
description: Leia as propriedades e os relacionamentos do objeto mobileAppIntentAndState.
ms.openlocfilehash: 837165f713aea00061b721a41003adc479a46b4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035700"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="875be-103">Obter mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="875be-103">Get mobileAppIntentAndState</span></span>

> <span data-ttu-id="875be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="875be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="875be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="875be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="875be-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="875be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="875be-107">Leia as propriedades e os relacionamentos do objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="875be-107">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="875be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="875be-108">Prerequisites</span></span>
<span data-ttu-id="875be-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="875be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="875be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="875be-111">Permission type</span></span>|<span data-ttu-id="875be-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="875be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="875be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="875be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="875be-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="875be-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="875be-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="875be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="875be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="875be-116">Not supported.</span></span>|
|<span data-ttu-id="875be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="875be-117">Application</span></span>|<span data-ttu-id="875be-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="875be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="875be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="875be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="875be-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="875be-120">Optional query parameters</span></span>
<span data-ttu-id="875be-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="875be-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="875be-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="875be-122">Request headers</span></span>
|<span data-ttu-id="875be-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="875be-123">Header</span></span>|<span data-ttu-id="875be-124">Valor</span><span class="sxs-lookup"><span data-stu-id="875be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="875be-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="875be-125">Authorization</span></span>|<span data-ttu-id="875be-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="875be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="875be-127">Accept</span><span class="sxs-lookup"><span data-stu-id="875be-127">Accept</span></span>|<span data-ttu-id="875be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="875be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="875be-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="875be-129">Request body</span></span>
<span data-ttu-id="875be-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="875be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="875be-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="875be-131">Response</span></span>
<span data-ttu-id="875be-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="875be-132">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="875be-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="875be-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="875be-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="875be-134">Request</span></span>
<span data-ttu-id="875be-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="875be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="875be-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="875be-136">Response</span></span>
<span data-ttu-id="875be-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="875be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





