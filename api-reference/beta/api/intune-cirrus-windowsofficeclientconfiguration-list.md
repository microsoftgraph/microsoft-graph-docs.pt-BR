---
title: Listar windowsOfficeClientConfigurations
description: Listar Propriedades e relações dos objetos windowsOfficeClientConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa8f786ed4ae7535d629c20e1e9f5712f0b29e38
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48714882"
---
# <a name="list-windowsofficeclientconfigurations"></a><span data-ttu-id="5b6ac-103">Listar windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="5b6ac-103">List windowsOfficeClientConfigurations</span></span>

<span data-ttu-id="5b6ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b6ac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b6ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b6ac-107">Listar Propriedades e relações dos objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5b6ac-107">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b6ac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b6ac-108">Prerequisites</span></span>
<span data-ttu-id="5b6ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b6ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b6ac-111">Permission type</span></span>|<span data-ttu-id="5b6ac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b6ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b6ac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b6ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b6ac-114">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="5b6ac-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b6ac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b6ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b6ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-116">Not supported.</span></span>|
|<span data-ttu-id="5b6ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b6ac-117">Application</span></span>|<span data-ttu-id="5b6ac-118">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="5b6ac-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b6ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5b6ac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6ac-120">Request headers</span></span>
|<span data-ttu-id="5b6ac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b6ac-121">Header</span></span>|<span data-ttu-id="5b6ac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5b6ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b6ac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b6ac-123">Authorization</span></span>|<span data-ttu-id="5b6ac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b6ac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b6ac-125">Accept</span></span>|<span data-ttu-id="5b6ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b6ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b6ac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6ac-127">Request body</span></span>
<span data-ttu-id="5b6ac-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b6ac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6ac-129">Response</span></span>
<span data-ttu-id="5b6ac-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b6ac-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b6ac-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b6ac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6ac-132">Request</span></span>
<span data-ttu-id="5b6ac-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="5b6ac-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6ac-134">Response</span></span>
<span data-ttu-id="5b6ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b6ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





