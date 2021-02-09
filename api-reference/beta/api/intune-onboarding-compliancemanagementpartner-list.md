---
title: Listar complianceManagementPartners
description: Listar propriedades e relações dos objetos complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1719a928918cd815da1af375026a7edbeb6b5802
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156893"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="5e0a9-103">Listar complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="5e0a9-103">List complianceManagementPartners</span></span>

<span data-ttu-id="5e0a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e0a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e0a9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e0a9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e0a9-107">Listar propriedades e relações dos [objetos complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="5e0a9-107">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e0a9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e0a9-108">Prerequisites</span></span>
<span data-ttu-id="5e0a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e0a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e0a9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e0a9-111">Permission type</span></span>|<span data-ttu-id="5e0a9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e0a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e0a9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e0a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e0a9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e0a9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5e0a9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e0a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e0a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-116">Not supported.</span></span>|
|<span data-ttu-id="5e0a9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e0a9-117">Application</span></span>|<span data-ttu-id="5e0a9-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e0a9-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e0a9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e0a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="5e0a9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e0a9-120">Request headers</span></span>
|<span data-ttu-id="5e0a9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e0a9-121">Header</span></span>|<span data-ttu-id="5e0a9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5e0a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e0a9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e0a9-123">Authorization</span></span>|<span data-ttu-id="5e0a9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e0a9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e0a9-125">Accept</span></span>|<span data-ttu-id="5e0a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e0a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e0a9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e0a9-127">Request body</span></span>
<span data-ttu-id="5e0a9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e0a9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e0a9-129">Response</span></span>
<span data-ttu-id="5e0a9-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-130">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e0a9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e0a9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e0a9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e0a9-132">Request</span></span>
<span data-ttu-id="5e0a9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="5e0a9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e0a9-134">Response</span></span>
<span data-ttu-id="5e0a9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e0a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2510

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
  ]
}
```




