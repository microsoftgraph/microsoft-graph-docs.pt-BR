---
title: Listar complianceManagementPartners
description: Listar propriedades e relações dos objetos complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a67f425e110def02b995b9fe24b218b35f28e88
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759062"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="10c6c-103">Listar complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="10c6c-103">List complianceManagementPartners</span></span>

<span data-ttu-id="10c6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10c6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10c6c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10c6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10c6c-106">Listar propriedades e relações dos [objetos complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="10c6c-106">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10c6c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10c6c-107">Prerequisites</span></span>
<span data-ttu-id="10c6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10c6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10c6c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10c6c-110">Permission type</span></span>|<span data-ttu-id="10c6c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10c6c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10c6c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10c6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10c6c-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c6c-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10c6c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10c6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10c6c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10c6c-115">Not supported.</span></span>|
|<span data-ttu-id="10c6c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10c6c-116">Application</span></span>|<span data-ttu-id="10c6c-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c6c-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10c6c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10c6c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="10c6c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10c6c-119">Request headers</span></span>
|<span data-ttu-id="10c6c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10c6c-120">Header</span></span>|<span data-ttu-id="10c6c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10c6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10c6c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10c6c-122">Authorization</span></span>|<span data-ttu-id="10c6c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10c6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10c6c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10c6c-124">Accept</span></span>|<span data-ttu-id="10c6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10c6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10c6c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10c6c-126">Request body</span></span>
<span data-ttu-id="10c6c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10c6c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10c6c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="10c6c-128">Response</span></span>
<span data-ttu-id="10c6c-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10c6c-129">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10c6c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10c6c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="10c6c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10c6c-131">Request</span></span>
<span data-ttu-id="10c6c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10c6c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="10c6c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="10c6c-133">Response</span></span>
<span data-ttu-id="10c6c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10c6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.complianceManagementPartner",
      "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "displayName": "Display Name value",
      "macOsOnboarded": true,
      "androidOnboarded": true,
      "iosOnboarded": true,
      "macOsEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "androidEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "iosEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ]
    }
  ]
}
```




