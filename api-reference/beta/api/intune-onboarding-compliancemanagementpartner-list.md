---
title: Listar complianceManagementPartners
description: Listar Propriedades e relações dos objetos complianceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e72cb1c24f8d44516ef4cd8c6e9364ffbadfe5b5
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086687"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="fc3ae-103">Listar complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="fc3ae-103">List complianceManagementPartners</span></span>

> <span data-ttu-id="fc3ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc3ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc3ae-106">Listar Propriedades e relações dos objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="fc3ae-106">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc3ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc3ae-107">Prerequisites</span></span>
<span data-ttu-id="fc3ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc3ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc3ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc3ae-110">Permission type</span></span>|<span data-ttu-id="fc3ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc3ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc3ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc3ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc3ae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc3ae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fc3ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc3ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc3ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-115">Not supported.</span></span>|
|<span data-ttu-id="fc3ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc3ae-116">Application</span></span>|<span data-ttu-id="fc3ae-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc3ae-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc3ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="fc3ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ae-119">Request headers</span></span>
|<span data-ttu-id="fc3ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc3ae-120">Header</span></span>|<span data-ttu-id="fc3ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fc3ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc3ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc3ae-122">Authorization</span></span>|<span data-ttu-id="fc3ae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc3ae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc3ae-124">Accept</span></span>|<span data-ttu-id="fc3ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc3ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc3ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ae-126">Request body</span></span>
<span data-ttu-id="fc3ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc3ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3ae-128">Response</span></span>
<span data-ttu-id="fc3ae-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-129">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc3ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc3ae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc3ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3ae-131">Request</span></span>
<span data-ttu-id="fc3ae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="fc3ae-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3ae-133">Response</span></span>
<span data-ttu-id="fc3ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc3ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1490

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
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
          }
        }
      ],
      "windowsEnrollmentAssignments": [
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






