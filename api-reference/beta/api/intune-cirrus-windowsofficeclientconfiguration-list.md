---
title: Lista windowsOfficeClientConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windowsOfficeClientConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e66ee83bb08bf7b5c7f5eeb1b641571c70b99074
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409836"
---
# <a name="list-windowsofficeclientconfigurations"></a><span data-ttu-id="22465-103">Lista windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="22465-103">List windowsOfficeClientConfigurations</span></span>

> <span data-ttu-id="22465-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="22465-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22465-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22465-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22465-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="22465-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22465-107">Lista as propriedades e os relacionamentos dos objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="22465-107">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22465-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22465-108">Prerequisites</span></span>
<span data-ttu-id="22465-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22465-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22465-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22465-111">Permission type</span></span>|<span data-ttu-id="22465-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22465-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22465-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22465-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22465-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22465-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22465-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22465-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22465-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22465-116">Not supported.</span></span>|
|<span data-ttu-id="22465-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22465-117">Application</span></span>|<span data-ttu-id="22465-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22465-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22465-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22465-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22465-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22465-120">Request headers</span></span>
|<span data-ttu-id="22465-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22465-121">Header</span></span>|<span data-ttu-id="22465-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22465-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22465-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22465-123">Authorization</span></span>|<span data-ttu-id="22465-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22465-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22465-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22465-125">Accept</span></span>|<span data-ttu-id="22465-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22465-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22465-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22465-127">Request body</span></span>
<span data-ttu-id="22465-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22465-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22465-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="22465-129">Response</span></span>
<span data-ttu-id="22465-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22465-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22465-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22465-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="22465-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22465-132">Request</span></span>
<span data-ttu-id="22465-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22465-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="22465-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="22465-134">Response</span></span>
<span data-ttu-id="22465-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22465-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



