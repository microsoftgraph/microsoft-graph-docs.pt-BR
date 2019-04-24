---
title: Listar officeClientConfigurations
description: Obtenha todas as políticas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dbbfae2a7568977c8dbdbc640d0829837c5e3fb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483149"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="09a9d-103">Listar officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="09a9d-103">List officeClientConfigurations</span></span>

> <span data-ttu-id="09a9d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09a9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09a9d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09a9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09a9d-106">Obtenha todas as políticas.</span><span class="sxs-lookup"><span data-stu-id="09a9d-106">Get all policies.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09a9d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09a9d-107">Prerequisites</span></span>
<span data-ttu-id="09a9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09a9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09a9d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09a9d-110">Permission type</span></span>|<span data-ttu-id="09a9d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09a9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09a9d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09a9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09a9d-113">DeviceManagementConfiguration. ReadWrite. All DeviceManagementConfiguration. Read. All</span><span class="sxs-lookup"><span data-stu-id="09a9d-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="09a9d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09a9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09a9d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09a9d-115">Not supported.</span></span>|
|<span data-ttu-id="09a9d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09a9d-116">Application</span></span>|<span data-ttu-id="09a9d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09a9d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09a9d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09a9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="09a9d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09a9d-119">Request headers</span></span>
|<span data-ttu-id="09a9d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09a9d-120">Header</span></span>|<span data-ttu-id="09a9d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="09a9d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09a9d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="09a9d-122">Authorization</span></span>|<span data-ttu-id="09a9d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09a9d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09a9d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09a9d-124">Accept</span></span>|<span data-ttu-id="09a9d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09a9d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09a9d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09a9d-126">Request body</span></span>
<span data-ttu-id="09a9d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09a9d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09a9d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="09a9d-128">Response</span></span>
<span data-ttu-id="09a9d-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09a9d-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09a9d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09a9d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="09a9d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09a9d-131">Request</span></span>
<span data-ttu-id="09a9d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09a9d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="09a9d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="09a9d-133">Response</span></span>
<span data-ttu-id="09a9d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09a9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1207

{
  "value": [
    {
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
  ]
}
```



