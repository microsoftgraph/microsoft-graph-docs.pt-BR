---
title: Obter Conjuntoofficeclientconfiguration
description: Obtenha uma política específica.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a7e85b29a5f60b8a12bd5c26635d71aa4c397fe
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760302"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="23126-103">Obter Conjuntoofficeclientconfiguration</span><span class="sxs-lookup"><span data-stu-id="23126-103">Get officeClientConfiguration</span></span>

> <span data-ttu-id="23126-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23126-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23126-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23126-106">Obtenha uma política específica.</span><span class="sxs-lookup"><span data-stu-id="23126-106">Get a specific policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23126-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23126-107">Prerequisites</span></span>
<span data-ttu-id="23126-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23126-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23126-110">Permission type</span></span>|<span data-ttu-id="23126-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23126-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23126-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23126-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23126-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="23126-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="23126-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23126-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23126-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23126-115">Not supported.</span></span>|
|<span data-ttu-id="23126-116">Application</span><span class="sxs-lookup"><span data-stu-id="23126-116">Application</span></span>|<span data-ttu-id="23126-117">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="23126-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23126-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23126-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23126-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23126-119">Optional query parameters</span></span>
<span data-ttu-id="23126-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23126-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23126-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23126-121">Request headers</span></span>
|<span data-ttu-id="23126-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23126-122">Header</span></span>|<span data-ttu-id="23126-123">Valor</span><span class="sxs-lookup"><span data-stu-id="23126-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23126-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="23126-124">Authorization</span></span>|<span data-ttu-id="23126-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23126-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23126-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23126-126">Accept</span></span>|<span data-ttu-id="23126-127">application/json</span><span class="sxs-lookup"><span data-stu-id="23126-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23126-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23126-128">Request body</span></span>
<span data-ttu-id="23126-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23126-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23126-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="23126-130">Response</span></span>
<span data-ttu-id="23126-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23126-131">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23126-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23126-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="23126-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23126-133">Request</span></span>
<span data-ttu-id="23126-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23126-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="23126-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="23126-135">Response</span></span>
<span data-ttu-id="23126-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23126-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




