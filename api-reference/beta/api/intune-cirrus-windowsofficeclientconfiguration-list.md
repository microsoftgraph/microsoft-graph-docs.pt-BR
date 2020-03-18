---
title: Listar windowsOfficeClientConfigurations
description: Listar Propriedades e relações dos objetos windowsOfficeClientConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b59828b2605fffbfd6e8a0c7341a4d3c9de093a2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760225"
---
# <a name="list-windowsofficeclientconfigurations"></a><span data-ttu-id="1c364-103">Listar windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="1c364-103">List windowsOfficeClientConfigurations</span></span>

> <span data-ttu-id="1c364-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c364-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c364-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c364-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c364-106">Listar Propriedades e relações dos objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1c364-106">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c364-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c364-107">Prerequisites</span></span>
<span data-ttu-id="1c364-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c364-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c364-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c364-110">Permission type</span></span>|<span data-ttu-id="1c364-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c364-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c364-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c364-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c364-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="1c364-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c364-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c364-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c364-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c364-115">Not supported.</span></span>|
|<span data-ttu-id="1c364-116">Application</span><span class="sxs-lookup"><span data-stu-id="1c364-116">Application</span></span>|<span data-ttu-id="1c364-117">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="1c364-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c364-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c364-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c364-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c364-119">Request headers</span></span>
|<span data-ttu-id="1c364-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c364-120">Header</span></span>|<span data-ttu-id="1c364-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1c364-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c364-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c364-122">Authorization</span></span>|<span data-ttu-id="1c364-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c364-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c364-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c364-124">Accept</span></span>|<span data-ttu-id="1c364-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c364-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c364-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c364-126">Request body</span></span>
<span data-ttu-id="1c364-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c364-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c364-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c364-128">Response</span></span>
<span data-ttu-id="1c364-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c364-129">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c364-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c364-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c364-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c364-131">Request</span></span>
<span data-ttu-id="1c364-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c364-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="1c364-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c364-133">Response</span></span>
<span data-ttu-id="1c364-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c364-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1214

{
  "value": [
    {
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
  ]
}
```




