---
title: Obter windowsOfficeClientSecurityConfiguration
description: Obtenha um objeto de windowsOfficeClientSecurityConfiguration de diretiva de segurança específicos.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a1619e7e1ed30afbc6b04f168f8e1fda2456e749
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409570"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="22f70-103">Obter windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="22f70-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="22f70-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="22f70-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22f70-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22f70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22f70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="22f70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f70-107">Obtenha um objeto de [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) de diretiva de segurança específicos.</span><span class="sxs-lookup"><span data-stu-id="22f70-107">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22f70-108">Prerequisites</span></span>
<span data-ttu-id="22f70-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22f70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22f70-111">Permission type</span></span>|<span data-ttu-id="22f70-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22f70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f70-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22f70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22f70-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22f70-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22f70-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22f70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f70-116">Not supported.</span></span>|
|<span data-ttu-id="22f70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22f70-117">Application</span></span>|<span data-ttu-id="22f70-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f70-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22f70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22f70-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22f70-120">Optional query parameters</span></span>
<span data-ttu-id="22f70-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22f70-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22f70-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22f70-122">Request headers</span></span>
|<span data-ttu-id="22f70-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22f70-123">Header</span></span>|<span data-ttu-id="22f70-124">Valor</span><span class="sxs-lookup"><span data-stu-id="22f70-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f70-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="22f70-125">Authorization</span></span>|<span data-ttu-id="22f70-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22f70-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f70-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22f70-127">Accept</span></span>|<span data-ttu-id="22f70-128">application/json</span><span class="sxs-lookup"><span data-stu-id="22f70-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f70-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22f70-129">Request body</span></span>
<span data-ttu-id="22f70-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22f70-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22f70-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f70-131">Response</span></span>
<span data-ttu-id="22f70-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22f70-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f70-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22f70-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f70-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22f70-134">Request</span></span>
<span data-ttu-id="22f70-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22f70-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="22f70-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f70-136">Response</span></span>
<span data-ttu-id="22f70-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22f70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



