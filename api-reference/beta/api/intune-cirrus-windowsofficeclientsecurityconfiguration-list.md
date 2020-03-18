---
title: Listar windowsOfficeClientSecurityConfigurations
description: Listar Propriedades e relações dos objetos windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6485a05e93acb053b40c9ad53cfb3f278209ef0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760190"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="e1faa-103">Listar windowsOfficeClientSecurityConfigurations</span><span class="sxs-lookup"><span data-stu-id="e1faa-103">List windowsOfficeClientSecurityConfigurations</span></span>

> <span data-ttu-id="e1faa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1faa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1faa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1faa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1faa-106">Listar Propriedades e relações dos objetos [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e1faa-106">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1faa-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1faa-107">Prerequisites</span></span>
<span data-ttu-id="e1faa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1faa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1faa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1faa-110">Permission type</span></span>|<span data-ttu-id="e1faa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1faa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1faa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1faa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1faa-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="e1faa-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e1faa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1faa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1faa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1faa-115">Not supported.</span></span>|
|<span data-ttu-id="e1faa-116">Application</span><span class="sxs-lookup"><span data-stu-id="e1faa-116">Application</span></span>|<span data-ttu-id="e1faa-117">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="e1faa-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1faa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1faa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e1faa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1faa-119">Request headers</span></span>
|<span data-ttu-id="e1faa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1faa-120">Header</span></span>|<span data-ttu-id="e1faa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1faa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1faa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1faa-122">Authorization</span></span>|<span data-ttu-id="e1faa-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1faa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1faa-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1faa-124">Accept</span></span>|<span data-ttu-id="e1faa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1faa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1faa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1faa-126">Request body</span></span>
<span data-ttu-id="e1faa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1faa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1faa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1faa-128">Response</span></span>
<span data-ttu-id="e1faa-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1faa-129">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1faa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1faa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1faa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1faa-131">Request</span></span>
<span data-ttu-id="e1faa-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1faa-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="e1faa-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1faa-133">Response</span></span>
<span data-ttu-id="e1faa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1faa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1222

{
  "value": [
    {
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
  ]
}
```




