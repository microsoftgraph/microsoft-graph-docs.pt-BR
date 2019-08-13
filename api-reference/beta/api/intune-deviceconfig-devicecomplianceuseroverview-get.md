---
title: Acessar deviceComplianceUserOverview
description: Leia as propriedades e relações de objetos de deviceComplianceUserOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8cde410a149b88f440ba2761bf8b8d274f9738f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346104"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="7089f-103">Acessar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="7089f-103">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="7089f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7089f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7089f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7089f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7089f-106">Leia as propriedades e relações de objetos de [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="7089f-106">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7089f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7089f-107">Prerequisites</span></span>
<span data-ttu-id="7089f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7089f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7089f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7089f-110">Permission type</span></span>|<span data-ttu-id="7089f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7089f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7089f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7089f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7089f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7089f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7089f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7089f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7089f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7089f-115">Not supported.</span></span>|
|<span data-ttu-id="7089f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7089f-116">Application</span></span>|<span data-ttu-id="7089f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7089f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7089f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7089f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7089f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7089f-119">Optional query parameters</span></span>
<span data-ttu-id="7089f-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7089f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7089f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7089f-121">Request headers</span></span>
|<span data-ttu-id="7089f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7089f-122">Header</span></span>|<span data-ttu-id="7089f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7089f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7089f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7089f-124">Authorization</span></span>|<span data-ttu-id="7089f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7089f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7089f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7089f-126">Accept</span></span>|<span data-ttu-id="7089f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7089f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7089f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7089f-128">Request body</span></span>
<span data-ttu-id="7089f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7089f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7089f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7089f-130">Response</span></span>
<span data-ttu-id="7089f-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7089f-131">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7089f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7089f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7089f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7089f-133">Request</span></span>
<span data-ttu-id="7089f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7089f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="7089f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7089f-135">Response</span></span>
<span data-ttu-id="7089f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7089f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
    "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```






