---
title: Obter officeClientConfiguration
description: Obter uma política específica.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3b4a2f582d093798145d971936ac3510813ccb0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665651"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="54ba4-103">Obter officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="54ba4-103">Get officeClientConfiguration</span></span>

<span data-ttu-id="54ba4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54ba4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54ba4-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54ba4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54ba4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54ba4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54ba4-107">Obter uma política específica.</span><span class="sxs-lookup"><span data-stu-id="54ba4-107">Get a specific policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54ba4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54ba4-108">Prerequisites</span></span>
<span data-ttu-id="54ba4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54ba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54ba4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54ba4-111">Permission type</span></span>|<span data-ttu-id="54ba4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54ba4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54ba4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54ba4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54ba4-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="54ba4-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="54ba4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54ba4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54ba4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54ba4-116">Not supported.</span></span>|
|<span data-ttu-id="54ba4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54ba4-117">Application</span></span>|<span data-ttu-id="54ba4-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="54ba4-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54ba4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54ba4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54ba4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54ba4-120">Optional query parameters</span></span>
<span data-ttu-id="54ba4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54ba4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="54ba4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54ba4-122">Request headers</span></span>
|<span data-ttu-id="54ba4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54ba4-123">Header</span></span>|<span data-ttu-id="54ba4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="54ba4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54ba4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="54ba4-125">Authorization</span></span>|<span data-ttu-id="54ba4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54ba4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54ba4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54ba4-127">Accept</span></span>|<span data-ttu-id="54ba4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="54ba4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54ba4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54ba4-129">Request body</span></span>
<span data-ttu-id="54ba4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54ba4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54ba4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="54ba4-131">Response</span></span>
<span data-ttu-id="54ba4-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54ba4-132">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54ba4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54ba4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="54ba4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54ba4-134">Request</span></span>
<span data-ttu-id="54ba4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54ba4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="54ba4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="54ba4-136">Response</span></span>
<span data-ttu-id="54ba4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54ba4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




