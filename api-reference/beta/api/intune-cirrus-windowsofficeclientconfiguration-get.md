---
title: Obter windowsOfficeClientConfiguration
description: Obtenha um objeto windowsOfficeClientConfiguration de política de não segurança específico.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e8c847d884b34a4077052210581b194edbf8511
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444403"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="ddfe6-103">Obter windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddfe6-103">Get windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="ddfe6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ddfe6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddfe6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddfe6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddfe6-107">Obtenha um objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) de política de não segurança específico.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-107">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddfe6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddfe6-108">Prerequisites</span></span>
<span data-ttu-id="ddfe6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddfe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddfe6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddfe6-111">Permission type</span></span>|<span data-ttu-id="ddfe6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddfe6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddfe6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddfe6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddfe6-114">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="ddfe6-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ddfe6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddfe6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddfe6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-116">Not supported.</span></span>|
|<span data-ttu-id="ddfe6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddfe6-117">Application</span></span>|<span data-ttu-id="ddfe6-118">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="ddfe6-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddfe6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddfe6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddfe6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddfe6-120">Optional query parameters</span></span>
<span data-ttu-id="ddfe6-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddfe6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfe6-122">Request headers</span></span>
|<span data-ttu-id="ddfe6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddfe6-123">Header</span></span>|<span data-ttu-id="ddfe6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ddfe6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddfe6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddfe6-125">Authorization</span></span>|<span data-ttu-id="ddfe6-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddfe6-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ddfe6-127">Accept</span></span>|<span data-ttu-id="ddfe6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ddfe6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddfe6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfe6-129">Request body</span></span>
<span data-ttu-id="ddfe6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddfe6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfe6-131">Response</span></span>
<span data-ttu-id="ddfe6-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddfe6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddfe6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddfe6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfe6-134">Request</span></span>
<span data-ttu-id="ddfe6-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="ddfe6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfe6-136">Response</span></span>
<span data-ttu-id="ddfe6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddfe6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





