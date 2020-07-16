---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 417f392126f521d1e5d3464652c7608e7a31ca8b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791809"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="adfdc-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="adfdc-103">List deviceManagementPartners</span></span>

<span data-ttu-id="adfdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adfdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adfdc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="adfdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adfdc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="adfdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adfdc-107">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="adfdc-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adfdc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="adfdc-108">Prerequisites</span></span>
<span data-ttu-id="adfdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adfdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adfdc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adfdc-111">Permission type</span></span>|<span data-ttu-id="adfdc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="adfdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adfdc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adfdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adfdc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="adfdc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="adfdc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adfdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adfdc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adfdc-116">Not supported.</span></span>|
|<span data-ttu-id="adfdc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adfdc-117">Application</span></span>|<span data-ttu-id="adfdc-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="adfdc-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adfdc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adfdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="adfdc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adfdc-120">Request headers</span></span>
|<span data-ttu-id="adfdc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="adfdc-121">Header</span></span>|<span data-ttu-id="adfdc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="adfdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adfdc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="adfdc-123">Authorization</span></span>|<span data-ttu-id="adfdc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adfdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adfdc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="adfdc-125">Accept</span></span>|<span data-ttu-id="adfdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adfdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adfdc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adfdc-127">Request body</span></span>
<span data-ttu-id="adfdc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="adfdc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adfdc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="adfdc-129">Response</span></span>
<span data-ttu-id="adfdc-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adfdc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adfdc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adfdc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="adfdc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adfdc-132">Request</span></span>
<span data-ttu-id="adfdc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adfdc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="adfdc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="adfdc-134">Response</span></span>
<span data-ttu-id="adfdc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adfdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



