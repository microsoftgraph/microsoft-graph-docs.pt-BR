---
title: Obter complianceManagementPartner
description: Leia as propriedades e as relações do objeto complianceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f88054b46668016b3fda0e7e7733479863ec163
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086694"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="a6274-103">Obter complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a6274-103">Get complianceManagementPartner</span></span>

> <span data-ttu-id="a6274-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6274-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6274-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6274-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6274-106">Leia as propriedades e as relações do objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="a6274-106">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6274-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6274-107">Prerequisites</span></span>
<span data-ttu-id="a6274-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6274-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6274-110">Permission type</span></span>|<span data-ttu-id="a6274-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6274-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6274-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6274-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6274-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6274-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a6274-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6274-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6274-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6274-115">Not supported.</span></span>|
|<span data-ttu-id="a6274-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6274-116">Application</span></span>|<span data-ttu-id="a6274-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6274-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6274-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6274-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6274-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6274-119">Optional query parameters</span></span>
<span data-ttu-id="a6274-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a6274-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6274-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6274-121">Request headers</span></span>
|<span data-ttu-id="a6274-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6274-122">Header</span></span>|<span data-ttu-id="a6274-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a6274-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6274-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6274-124">Authorization</span></span>|<span data-ttu-id="a6274-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6274-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6274-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6274-126">Accept</span></span>|<span data-ttu-id="a6274-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a6274-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6274-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6274-128">Request body</span></span>
<span data-ttu-id="a6274-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6274-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6274-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6274-130">Response</span></span>
<span data-ttu-id="a6274-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6274-131">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6274-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6274-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6274-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6274-133">Request</span></span>
<span data-ttu-id="a6274-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6274-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="a6274-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6274-135">Response</span></span>
<span data-ttu-id="a6274-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6274-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

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
}
```






