---
title: Listar complianceManagementPartners
description: Listar Propriedades e relações dos objetos complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 278a39402d03ab623abb55f7dce134212ae887e6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791837"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="87b10-103">Listar complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="87b10-103">List complianceManagementPartners</span></span>

<span data-ttu-id="87b10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87b10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87b10-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87b10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87b10-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87b10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87b10-107">Listar Propriedades e relações dos objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="87b10-107">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87b10-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87b10-108">Prerequisites</span></span>
<span data-ttu-id="87b10-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="87b10-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="87b10-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87b10-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87b10-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87b10-111">Permission type</span></span>|<span data-ttu-id="87b10-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87b10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87b10-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87b10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87b10-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="87b10-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="87b10-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87b10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87b10-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87b10-116">Not supported.</span></span>|
|<span data-ttu-id="87b10-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87b10-117">Application</span></span>|<span data-ttu-id="87b10-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="87b10-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87b10-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87b10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="87b10-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87b10-120">Request headers</span></span>
|<span data-ttu-id="87b10-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87b10-121">Header</span></span>|<span data-ttu-id="87b10-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87b10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87b10-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87b10-123">Authorization</span></span>|<span data-ttu-id="87b10-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87b10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87b10-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87b10-125">Accept</span></span>|<span data-ttu-id="87b10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87b10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87b10-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87b10-127">Request body</span></span>
<span data-ttu-id="87b10-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87b10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87b10-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="87b10-129">Response</span></span>
<span data-ttu-id="87b10-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87b10-130">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87b10-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87b10-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87b10-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87b10-132">Request</span></span>
<span data-ttu-id="87b10-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87b10-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="87b10-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87b10-134">Response</span></span>
<span data-ttu-id="87b10-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="87b10-135">Here is an example of the response.</span></span> <span data-ttu-id="87b10-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="87b10-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="87b10-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="87b10-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2222

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.complianceManagementPartner",
      "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "displayName": "Display Name value",
      "macOsOnboarded": true,
      "windowsOnboarded": true,
      "androidOnboarded": true,
      "iosOnboarded": true,
      "macOsEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include"
          }
        }
      ],
      "windowsEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include"
          }
        }
      ],
      "androidEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include"
          }
        }
      ],
      "iosEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
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



