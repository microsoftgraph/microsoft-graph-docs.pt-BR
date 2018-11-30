---
title: Lista windowsOfficeClientConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windowsOfficeClientConfiguration.
ms.openlocfilehash: 0e14dc2ede95d0b1b5fcb4830e47292d2d604f7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033274"
---
# <a name="list-windowsofficeclientconfigurations"></a><span data-ttu-id="34564-103">Lista windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="34564-103">List windowsOfficeClientConfigurations</span></span>

> <span data-ttu-id="34564-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34564-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34564-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34564-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34564-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="34564-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34564-107">Lista as propriedades e os relacionamentos dos objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="34564-107">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34564-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34564-108">Prerequisites</span></span>
<span data-ttu-id="34564-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34564-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34564-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34564-111">Permission type</span></span>|<span data-ttu-id="34564-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34564-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34564-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34564-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34564-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34564-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34564-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34564-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34564-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34564-116">Not supported.</span></span>|
|<span data-ttu-id="34564-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34564-117">Application</span></span>|<span data-ttu-id="34564-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34564-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34564-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34564-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34564-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34564-120">Request headers</span></span>
|<span data-ttu-id="34564-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34564-121">Header</span></span>|<span data-ttu-id="34564-122">Valor</span><span class="sxs-lookup"><span data-stu-id="34564-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34564-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34564-123">Authorization</span></span>|<span data-ttu-id="34564-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34564-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34564-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34564-125">Accept</span></span>|<span data-ttu-id="34564-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34564-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34564-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34564-127">Request body</span></span>
<span data-ttu-id="34564-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34564-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34564-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34564-129">Response</span></span>
<span data-ttu-id="34564-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34564-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34564-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34564-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="34564-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34564-132">Request</span></span>
<span data-ttu-id="34564-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34564-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="34564-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="34564-134">Response</span></span>
<span data-ttu-id="34564-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34564-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



