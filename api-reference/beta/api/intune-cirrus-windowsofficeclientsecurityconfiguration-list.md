---
title: Lista windowsOfficeClientSecurityConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 76bce73185c4ac68a4839c85978a3f4fadc7dcfe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408835"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="c061e-103">Lista windowsOfficeClientSecurityConfigurations</span><span class="sxs-lookup"><span data-stu-id="c061e-103">List windowsOfficeClientSecurityConfigurations</span></span>

> <span data-ttu-id="c061e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c061e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c061e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c061e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c061e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c061e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c061e-107">Lista as propriedades e os relacionamentos dos objetos [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c061e-107">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c061e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c061e-108">Prerequisites</span></span>
<span data-ttu-id="c061e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c061e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c061e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c061e-111">Permission type</span></span>|<span data-ttu-id="c061e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c061e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c061e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c061e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c061e-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c061e-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c061e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c061e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c061e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c061e-116">Not supported.</span></span>|
|<span data-ttu-id="c061e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c061e-117">Application</span></span>|<span data-ttu-id="c061e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c061e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c061e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c061e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c061e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c061e-120">Request headers</span></span>
|<span data-ttu-id="c061e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c061e-121">Header</span></span>|<span data-ttu-id="c061e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c061e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c061e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c061e-123">Authorization</span></span>|<span data-ttu-id="c061e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c061e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c061e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c061e-125">Accept</span></span>|<span data-ttu-id="c061e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c061e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c061e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c061e-127">Request body</span></span>
<span data-ttu-id="c061e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c061e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c061e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c061e-129">Response</span></span>
<span data-ttu-id="c061e-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c061e-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c061e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c061e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c061e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c061e-132">Request</span></span>
<span data-ttu-id="c061e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c061e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="c061e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c061e-134">Response</span></span>
<span data-ttu-id="c061e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c061e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



