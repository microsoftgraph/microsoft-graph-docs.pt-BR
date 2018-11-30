---
title: Obter officeClientConfiguration
description: Obtenha uma diretiva específica.
ms.openlocfilehash: 79be4463aa2278c0e3102c672777f02ae06cd17d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039706"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="4b2a4-103">Obter officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b2a4-103">Get officeClientConfiguration</span></span>

> <span data-ttu-id="4b2a4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b2a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b2a4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b2a4-107">Obtenha uma diretiva específica.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-107">Get a specific policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b2a4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b2a4-108">Prerequisites</span></span>
<span data-ttu-id="4b2a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b2a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b2a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b2a4-111">Permission type</span></span>|<span data-ttu-id="4b2a4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b2a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b2a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b2a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b2a4-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b2a4-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b2a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b2a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b2a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-116">Not supported.</span></span>|
|<span data-ttu-id="4b2a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b2a4-117">Application</span></span>|<span data-ttu-id="4b2a4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b2a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b2a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b2a4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4b2a4-120">Optional query parameters</span></span>
<span data-ttu-id="4b2a4-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4b2a4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b2a4-122">Request headers</span></span>
|<span data-ttu-id="4b2a4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b2a4-123">Header</span></span>|<span data-ttu-id="4b2a4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4b2a4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b2a4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b2a4-125">Authorization</span></span>|<span data-ttu-id="4b2a4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b2a4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4b2a4-127">Accept</span></span>|<span data-ttu-id="4b2a4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4b2a4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b2a4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b2a4-129">Request body</span></span>
<span data-ttu-id="4b2a4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b2a4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b2a4-131">Response</span></span>
<span data-ttu-id="4b2a4-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-132">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b2a4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b2a4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b2a4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b2a4-134">Request</span></span>
<span data-ttu-id="4b2a4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="4b2a4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b2a4-136">Response</span></span>
<span data-ttu-id="4b2a4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b2a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfiguration",
    "id": "362ce0f0-e0f0-362c-f0e0-2c36f0e02c36",
    "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
    "policyPayload": "<Unknown Primitive Type Edm.Stream>",
    "description": "Description value",
    "displayName": "Display Name value",
    "priority": 8,
    "userCheckinSummary": {
      "@odata.type": "microsoft.graph.officeUserCheckinSummary",
      "succeededUserCount": 2,
      "failedUserCount": 15
    },
    "checkinStatuses": [
      {
        "@odata.type": "microsoft.graph.officeClientCheckinStatus",
        "userPrincipalName": "User Principal Name value",
        "deviceName": "Device Name value",
        "devicePlatform": "Device Platform value",
        "devicePlatformVersion": "Device Platform Version value",
        "wasSuccessful": true,
        "userId": "User Id value",
        "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
        "errorMessage": "Error Message value",
        "appliedPolicies": [
          "Applied Policies value"
        ]
      }
    ]
  }
}
```



