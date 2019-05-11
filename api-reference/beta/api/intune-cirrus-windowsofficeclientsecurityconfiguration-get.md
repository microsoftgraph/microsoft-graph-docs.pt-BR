---
title: Obter windowsOfficeClientSecurityConfiguration
description: Obtenha um objeto windowsOfficeClientSecurityConfiguration de política de segurança específico.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 3c55e9d1018d2781bfbd4e761eafcf054485798a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933953"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="17e83-103">Obter windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="17e83-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="17e83-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17e83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17e83-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17e83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17e83-106">Obtenha um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) de política de segurança específico.</span><span class="sxs-lookup"><span data-stu-id="17e83-106">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17e83-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17e83-107">Prerequisites</span></span>
<span data-ttu-id="17e83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17e83-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17e83-110">Permission type</span></span>|<span data-ttu-id="17e83-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17e83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17e83-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17e83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17e83-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="17e83-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="17e83-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17e83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17e83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17e83-115">Not supported.</span></span>|
|<span data-ttu-id="17e83-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17e83-116">Application</span></span>|<span data-ttu-id="17e83-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17e83-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17e83-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17e83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17e83-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17e83-119">Optional query parameters</span></span>
<span data-ttu-id="17e83-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17e83-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17e83-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17e83-121">Request headers</span></span>
|<span data-ttu-id="17e83-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17e83-122">Header</span></span>|<span data-ttu-id="17e83-123">Valor</span><span class="sxs-lookup"><span data-stu-id="17e83-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17e83-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17e83-124">Authorization</span></span>|<span data-ttu-id="17e83-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17e83-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17e83-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17e83-126">Accept</span></span>|<span data-ttu-id="17e83-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17e83-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17e83-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17e83-128">Request body</span></span>
<span data-ttu-id="17e83-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17e83-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17e83-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e83-130">Response</span></span>
<span data-ttu-id="17e83-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17e83-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17e83-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17e83-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17e83-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17e83-133">Request</span></span>
<span data-ttu-id="17e83-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17e83-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="17e83-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e83-135">Response</span></span>
<span data-ttu-id="17e83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17e83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



