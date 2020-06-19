---
title: Obter complianceManagementPartner
description: Leia as propriedades e as relações do objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b4830f22ff6b37c279a348e02f115e7f98a461c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791844"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="98361-103">Obter complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="98361-103">Get complianceManagementPartner</span></span>

<span data-ttu-id="98361-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98361-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98361-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98361-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98361-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98361-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98361-107">Leia as propriedades e as relações do objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="98361-107">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98361-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98361-108">Prerequisites</span></span>
<span data-ttu-id="98361-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="98361-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="98361-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98361-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98361-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98361-111">Permission type</span></span>|<span data-ttu-id="98361-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98361-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98361-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98361-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98361-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="98361-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="98361-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98361-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98361-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98361-116">Not supported.</span></span>|
|<span data-ttu-id="98361-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98361-117">Application</span></span>|<span data-ttu-id="98361-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="98361-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98361-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98361-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98361-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="98361-120">Optional query parameters</span></span>
<span data-ttu-id="98361-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="98361-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98361-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98361-122">Request headers</span></span>
|<span data-ttu-id="98361-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98361-123">Header</span></span>|<span data-ttu-id="98361-124">Valor</span><span class="sxs-lookup"><span data-stu-id="98361-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98361-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="98361-125">Authorization</span></span>|<span data-ttu-id="98361-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98361-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98361-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98361-127">Accept</span></span>|<span data-ttu-id="98361-128">application/json</span><span class="sxs-lookup"><span data-stu-id="98361-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98361-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98361-129">Request body</span></span>
<span data-ttu-id="98361-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98361-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98361-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="98361-131">Response</span></span>
<span data-ttu-id="98361-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98361-132">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98361-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98361-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="98361-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98361-134">Request</span></span>
<span data-ttu-id="98361-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98361-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="98361-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="98361-136">Response</span></span>
<span data-ttu-id="98361-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="98361-137">Here is an example of the response.</span></span> <span data-ttu-id="98361-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="98361-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="98361-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="98361-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2110

{
  "value": {
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
}
```



