---
title: Listar windowsOfficeClientSecurityConfigurations
description: Listar propriedades e relações dos objetos windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0848de68aa9cb8d1fe86f226721bb7e09bd6ac4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751731"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="45ebd-103">Listar windowsOfficeClientSecurityConfigurations</span><span class="sxs-lookup"><span data-stu-id="45ebd-103">List windowsOfficeClientSecurityConfigurations</span></span>

<span data-ttu-id="45ebd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45ebd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45ebd-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45ebd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45ebd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45ebd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45ebd-107">Listar propriedades e relações dos [objetos windowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45ebd-107">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45ebd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45ebd-108">Prerequisites</span></span>
<span data-ttu-id="45ebd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45ebd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45ebd-111">Permission type</span></span>|<span data-ttu-id="45ebd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45ebd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45ebd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45ebd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45ebd-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ebd-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45ebd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45ebd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45ebd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45ebd-116">Not supported.</span></span>|
|<span data-ttu-id="45ebd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45ebd-117">Application</span></span>|<span data-ttu-id="45ebd-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ebd-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45ebd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45ebd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45ebd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45ebd-120">Request headers</span></span>
|<span data-ttu-id="45ebd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45ebd-121">Header</span></span>|<span data-ttu-id="45ebd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45ebd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45ebd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45ebd-123">Authorization</span></span>|<span data-ttu-id="45ebd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45ebd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45ebd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45ebd-125">Accept</span></span>|<span data-ttu-id="45ebd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45ebd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45ebd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45ebd-127">Request body</span></span>
<span data-ttu-id="45ebd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45ebd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45ebd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="45ebd-129">Response</span></span>
<span data-ttu-id="45ebd-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45ebd-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45ebd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45ebd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45ebd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45ebd-132">Request</span></span>
<span data-ttu-id="45ebd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45ebd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="45ebd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="45ebd-134">Response</span></span>
<span data-ttu-id="45ebd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45ebd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




