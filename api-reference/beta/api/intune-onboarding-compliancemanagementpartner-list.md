---
title: Listar complianceManagementPartners
description: Listar Propriedades e relações dos objetos complianceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 152ec1bee04a25a3d63ff34f58b63a1447d42946
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462443"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="a54a7-103">Listar complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="a54a7-103">List complianceManagementPartners</span></span>

<span data-ttu-id="a54a7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a54a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a54a7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a54a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a54a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a54a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a54a7-107">Listar Propriedades e relações dos objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="a54a7-107">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a54a7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a54a7-108">Prerequisites</span></span>
<span data-ttu-id="a54a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a54a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a54a7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a54a7-111">Permission type</span></span>|<span data-ttu-id="a54a7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a54a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a54a7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a54a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a54a7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a54a7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a54a7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a54a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a54a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a54a7-116">Not supported.</span></span>|
|<span data-ttu-id="a54a7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a54a7-117">Application</span></span>|<span data-ttu-id="a54a7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a54a7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a54a7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a54a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="a54a7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a54a7-120">Request headers</span></span>
|<span data-ttu-id="a54a7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a54a7-121">Header</span></span>|<span data-ttu-id="a54a7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a54a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a54a7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a54a7-123">Authorization</span></span>|<span data-ttu-id="a54a7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a54a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a54a7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a54a7-125">Accept</span></span>|<span data-ttu-id="a54a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a54a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a54a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a54a7-127">Request body</span></span>
<span data-ttu-id="a54a7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a54a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a54a7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a54a7-129">Response</span></span>
<span data-ttu-id="a54a7-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a54a7-130">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a54a7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a54a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a54a7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a54a7-132">Request</span></span>
<span data-ttu-id="a54a7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a54a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="a54a7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a54a7-134">Response</span></span>
<span data-ttu-id="a54a7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a54a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





