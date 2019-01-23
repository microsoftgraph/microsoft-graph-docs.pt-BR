---
title: Obter windowsOfficeClientConfiguration
description: Obtenha um objeto de windowsOfficeClientConfiguration políticas específicas de não relacionadas à segurança.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b95bdadf77b2a9a6636311df4be19444e9802f4a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394268"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="370fa-103">Obter windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="370fa-103">Get windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="370fa-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="370fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="370fa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="370fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="370fa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="370fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="370fa-107">Obtenha um objeto de [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) políticas específicas de não relacionadas à segurança.</span><span class="sxs-lookup"><span data-stu-id="370fa-107">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="370fa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="370fa-108">Prerequisites</span></span>
<span data-ttu-id="370fa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="370fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="370fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="370fa-111">Permission type</span></span>|<span data-ttu-id="370fa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="370fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="370fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="370fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="370fa-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="370fa-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="370fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="370fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="370fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="370fa-116">Not supported.</span></span>|
|<span data-ttu-id="370fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="370fa-117">Application</span></span>|<span data-ttu-id="370fa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="370fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="370fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="370fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="370fa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="370fa-120">Optional query parameters</span></span>
<span data-ttu-id="370fa-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="370fa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="370fa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="370fa-122">Request headers</span></span>
|<span data-ttu-id="370fa-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="370fa-123">Header</span></span>|<span data-ttu-id="370fa-124">Valor</span><span class="sxs-lookup"><span data-stu-id="370fa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="370fa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="370fa-125">Authorization</span></span>|<span data-ttu-id="370fa-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="370fa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="370fa-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="370fa-127">Accept</span></span>|<span data-ttu-id="370fa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="370fa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="370fa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="370fa-129">Request body</span></span>
<span data-ttu-id="370fa-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="370fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="370fa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="370fa-131">Response</span></span>
<span data-ttu-id="370fa-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="370fa-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="370fa-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="370fa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="370fa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="370fa-134">Request</span></span>
<span data-ttu-id="370fa-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="370fa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="370fa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="370fa-136">Response</span></span>
<span data-ttu-id="370fa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="370fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1144

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
    "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
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



