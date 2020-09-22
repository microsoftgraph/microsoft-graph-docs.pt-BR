---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9813361f4748d260a8b9cd503f9430fed1a6c7da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000032"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="70882-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="70882-103">List deviceManagementPartners</span></span>

<span data-ttu-id="70882-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70882-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70882-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70882-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70882-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70882-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70882-107">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="70882-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70882-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70882-108">Prerequisites</span></span>
<span data-ttu-id="70882-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70882-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70882-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70882-111">Permission type</span></span>|<span data-ttu-id="70882-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70882-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70882-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70882-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70882-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="70882-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="70882-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70882-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70882-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70882-116">Not supported.</span></span>|
|<span data-ttu-id="70882-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70882-117">Application</span></span>|<span data-ttu-id="70882-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="70882-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70882-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70882-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="70882-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70882-120">Request headers</span></span>
|<span data-ttu-id="70882-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70882-121">Header</span></span>|<span data-ttu-id="70882-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70882-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70882-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70882-123">Authorization</span></span>|<span data-ttu-id="70882-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70882-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70882-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70882-125">Accept</span></span>|<span data-ttu-id="70882-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70882-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70882-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70882-127">Request body</span></span>
<span data-ttu-id="70882-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70882-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70882-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="70882-129">Response</span></span>
<span data-ttu-id="70882-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70882-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70882-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70882-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="70882-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70882-132">Request</span></span>
<span data-ttu-id="70882-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70882-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="70882-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="70882-134">Response</span></span>
<span data-ttu-id="70882-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70882-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1242

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
      "groupsRequiringPartnerEnrollment": [
        {
          "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include"
          }
        }
      ]
    }
  ]
}
```






