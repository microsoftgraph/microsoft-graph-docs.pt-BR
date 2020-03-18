---
title: Obter windowsOfficeClientSecurityConfiguration
description: Obtenha um objeto windowsOfficeClientSecurityConfiguration de política de segurança específico.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9634f41e84458c1a534168922c4e06830eb49ed3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760197"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="c9939-103">Obter windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9939-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="c9939-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9939-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9939-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9939-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9939-106">Obtenha um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) de política de segurança específico.</span><span class="sxs-lookup"><span data-stu-id="c9939-106">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9939-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9939-107">Prerequisites</span></span>
<span data-ttu-id="c9939-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9939-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9939-110">Permission type</span></span>|<span data-ttu-id="c9939-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9939-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9939-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9939-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9939-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="c9939-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9939-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9939-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9939-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9939-115">Not supported.</span></span>|
|<span data-ttu-id="c9939-116">Application</span><span class="sxs-lookup"><span data-stu-id="c9939-116">Application</span></span>|<span data-ttu-id="c9939-117">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="c9939-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9939-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9939-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9939-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9939-119">Optional query parameters</span></span>
<span data-ttu-id="c9939-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9939-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9939-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9939-121">Request headers</span></span>
|<span data-ttu-id="c9939-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9939-122">Header</span></span>|<span data-ttu-id="c9939-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c9939-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9939-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9939-124">Authorization</span></span>|<span data-ttu-id="c9939-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9939-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9939-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9939-126">Accept</span></span>|<span data-ttu-id="c9939-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c9939-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9939-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9939-128">Request body</span></span>
<span data-ttu-id="c9939-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9939-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9939-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9939-130">Response</span></span>
<span data-ttu-id="c9939-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9939-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9939-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9939-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9939-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9939-133">Request</span></span>
<span data-ttu-id="c9939-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9939-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="c9939-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9939-135">Response</span></span>
<span data-ttu-id="c9939-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9939-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




