---
title: Acessar deviceComplianceUserOverview
description: Leia as propriedades e relações de objetos de deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 340eef22071551195f6f89b3ffd37c81d4331932
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706769"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="d48d3-103">Acessar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="d48d3-103">Get deviceComplianceUserOverview</span></span>

<span data-ttu-id="d48d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d48d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d48d3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d48d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d48d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d48d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d48d3-107">Leia as propriedades e relações de objetos de [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="d48d3-107">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d48d3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d48d3-108">Prerequisites</span></span>
<span data-ttu-id="d48d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d48d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d48d3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d48d3-111">Permission type</span></span>|<span data-ttu-id="d48d3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d48d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d48d3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d48d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d48d3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d48d3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d48d3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d48d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d48d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d48d3-116">Not supported.</span></span>|
|<span data-ttu-id="d48d3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d48d3-117">Application</span></span>|<span data-ttu-id="d48d3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d48d3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d48d3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d48d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d48d3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d48d3-120">Optional query parameters</span></span>
<span data-ttu-id="d48d3-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d48d3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d48d3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d48d3-122">Request headers</span></span>
|<span data-ttu-id="d48d3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d48d3-123">Header</span></span>|<span data-ttu-id="d48d3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d48d3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d48d3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d48d3-125">Authorization</span></span>|<span data-ttu-id="d48d3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d48d3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d48d3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d48d3-127">Accept</span></span>|<span data-ttu-id="d48d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d48d3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d48d3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d48d3-129">Request body</span></span>
<span data-ttu-id="d48d3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d48d3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d48d3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d48d3-131">Response</span></span>
<span data-ttu-id="d48d3-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d48d3-132">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d48d3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d48d3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d48d3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d48d3-134">Request</span></span>
<span data-ttu-id="d48d3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d48d3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="d48d3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d48d3-136">Response</span></span>
<span data-ttu-id="d48d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d48d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





