---
title: Obter complianceManagementPartner
description: Ler propriedades e relações do objeto complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86ae121d11003fc2b6caa5730a43b124341a232a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152681"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="fcecc-103">Obter complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="fcecc-103">Get complianceManagementPartner</span></span>

<span data-ttu-id="fcecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcecc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcecc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fcecc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcecc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcecc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcecc-107">Ler propriedades e relações do [objeto complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="fcecc-107">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcecc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fcecc-108">Prerequisites</span></span>
<span data-ttu-id="fcecc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcecc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcecc-111">Permission type</span></span>|<span data-ttu-id="fcecc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcecc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcecc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcecc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcecc-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcecc-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fcecc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcecc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcecc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcecc-116">Not supported.</span></span>|
|<span data-ttu-id="fcecc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcecc-117">Application</span></span>|<span data-ttu-id="fcecc-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcecc-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcecc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcecc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcecc-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fcecc-120">Optional query parameters</span></span>
<span data-ttu-id="fcecc-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fcecc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcecc-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcecc-122">Request headers</span></span>
|<span data-ttu-id="fcecc-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fcecc-123">Header</span></span>|<span data-ttu-id="fcecc-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fcecc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcecc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcecc-125">Authorization</span></span>|<span data-ttu-id="fcecc-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcecc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcecc-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fcecc-127">Accept</span></span>|<span data-ttu-id="fcecc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fcecc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcecc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcecc-129">Request body</span></span>
<span data-ttu-id="fcecc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcecc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcecc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcecc-131">Response</span></span>
<span data-ttu-id="fcecc-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcecc-132">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcecc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcecc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcecc-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcecc-134">Request</span></span>
<span data-ttu-id="fcecc-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcecc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="fcecc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcecc-136">Response</span></span>
<span data-ttu-id="fcecc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcecc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2390

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
          "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include",
          "collectionId": "Collection Id value"
        }
      }
    ],
    "windowsEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include",
          "collectionId": "Collection Id value"
        }
      }
    ],
    "androidEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include",
          "collectionId": "Collection Id value"
        }
      }
    ],
    "iosEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include",
          "collectionId": "Collection Id value"
        }
      }
    ]
  }
}
```




