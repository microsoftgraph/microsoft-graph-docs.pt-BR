---
title: Obter windowsOfficeClientSecurityConfiguration
description: Obtenha um objeto windowsOfficeClientSecurityConfiguration de política de segurança específico.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 02edba061958739dd0dac43151e027b414be19d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152162"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="f2669-103">Obter windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2669-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="f2669-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2669-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2669-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2669-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2669-106">Obtenha um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) de política de segurança específico.</span><span class="sxs-lookup"><span data-stu-id="f2669-106">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2669-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2669-107">Prerequisites</span></span>
<span data-ttu-id="f2669-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2669-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2669-110">Permission type</span></span>|<span data-ttu-id="f2669-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2669-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2669-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2669-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2669-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="f2669-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2669-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2669-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2669-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2669-115">Not supported.</span></span>|
|<span data-ttu-id="f2669-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2669-116">Application</span></span>|<span data-ttu-id="f2669-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2669-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2669-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2669-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2669-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2669-119">Optional query parameters</span></span>
<span data-ttu-id="f2669-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2669-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2669-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2669-121">Request headers</span></span>
|<span data-ttu-id="f2669-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2669-122">Header</span></span>|<span data-ttu-id="f2669-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f2669-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2669-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2669-124">Authorization</span></span>|<span data-ttu-id="f2669-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2669-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2669-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2669-126">Accept</span></span>|<span data-ttu-id="f2669-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f2669-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2669-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2669-128">Request body</span></span>
<span data-ttu-id="f2669-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2669-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2669-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2669-130">Response</span></span>
<span data-ttu-id="f2669-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2669-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2669-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2669-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2669-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2669-133">Request</span></span>
<span data-ttu-id="f2669-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2669-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="f2669-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2669-135">Response</span></span>
<span data-ttu-id="f2669-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2669-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
    "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
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



