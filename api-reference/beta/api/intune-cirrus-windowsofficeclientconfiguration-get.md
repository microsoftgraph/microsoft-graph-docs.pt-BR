---
title: Obter windowsOfficeClientConfiguration
description: Obtenha um objeto windowsOfficeClientConfiguration de política de não segurança específico.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e1f34ead1df597a6b94df224398a6f6c2f77ab3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328225"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="0f279-103">Obter windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f279-103">Get windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="0f279-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f279-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f279-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f279-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f279-106">Obtenha um objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) de política de não segurança específico.</span><span class="sxs-lookup"><span data-stu-id="0f279-106">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f279-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f279-107">Prerequisites</span></span>
<span data-ttu-id="0f279-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f279-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f279-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f279-110">Permission type</span></span>|<span data-ttu-id="0f279-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f279-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f279-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f279-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f279-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="0f279-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f279-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f279-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f279-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f279-115">Not supported.</span></span>|
|<span data-ttu-id="0f279-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f279-116">Application</span></span>|<span data-ttu-id="0f279-117">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="0f279-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f279-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f279-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f279-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0f279-119">Optional query parameters</span></span>
<span data-ttu-id="0f279-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f279-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f279-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f279-121">Request headers</span></span>
|<span data-ttu-id="0f279-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f279-122">Header</span></span>|<span data-ttu-id="0f279-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0f279-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f279-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f279-124">Authorization</span></span>|<span data-ttu-id="0f279-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f279-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f279-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f279-126">Accept</span></span>|<span data-ttu-id="0f279-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0f279-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f279-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f279-128">Request body</span></span>
<span data-ttu-id="0f279-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f279-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f279-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f279-130">Response</span></span>
<span data-ttu-id="0f279-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f279-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f279-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f279-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f279-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f279-133">Request</span></span>
<span data-ttu-id="0f279-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f279-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="0f279-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f279-135">Response</span></span>
<span data-ttu-id="0f279-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f279-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






