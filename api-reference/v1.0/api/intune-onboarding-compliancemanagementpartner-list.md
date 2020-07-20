---
title: Listar complianceManagementPartners
description: Listar Propriedades e relações dos objetos complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91f43342fa21cad981663578ab0c98c3a2e1aefb
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744101"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="ffc23-103">Listar complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="ffc23-103">List complianceManagementPartners</span></span>

<span data-ttu-id="ffc23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffc23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffc23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ffc23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffc23-106">Listar Propriedades e relações dos objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="ffc23-106">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffc23-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ffc23-107">Prerequisites</span></span>
<span data-ttu-id="ffc23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffc23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffc23-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffc23-110">Permission type</span></span>|<span data-ttu-id="ffc23-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ffc23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffc23-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffc23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffc23-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffc23-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ffc23-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffc23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffc23-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffc23-115">Not supported.</span></span>|
|<span data-ttu-id="ffc23-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffc23-116">Application</span></span>|<span data-ttu-id="ffc23-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffc23-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffc23-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffc23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="ffc23-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffc23-119">Request headers</span></span>
|<span data-ttu-id="ffc23-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ffc23-120">Header</span></span>|<span data-ttu-id="ffc23-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ffc23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffc23-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffc23-122">Authorization</span></span>|<span data-ttu-id="ffc23-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffc23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffc23-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ffc23-124">Accept</span></span>|<span data-ttu-id="ffc23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffc23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffc23-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffc23-126">Request body</span></span>
<span data-ttu-id="ffc23-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ffc23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffc23-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffc23-128">Response</span></span>
<span data-ttu-id="ffc23-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffc23-129">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffc23-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffc23-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffc23-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffc23-131">Request</span></span>
<span data-ttu-id="ffc23-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffc23-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="ffc23-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffc23-133">Response</span></span>
<span data-ttu-id="ffc23-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ffc23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1192

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
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
          }
        }
      ],
      "androidEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
          }
        }
      ],
      "iosEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
          }
        }
      ]
    }
  ]
}
```



