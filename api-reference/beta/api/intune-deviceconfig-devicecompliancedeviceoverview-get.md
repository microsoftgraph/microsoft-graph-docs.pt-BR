---
title: Acessar deviceComplianceDeviceOverview
description: Leia as propriedades e as relações do objeto deviceComplianceDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0b0f6fc0ae16221f26075c39c204609805e4e39
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434228"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="5e062-103">Acessar deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5e062-103">Get deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="5e062-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e062-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e062-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e062-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e062-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e062-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e062-107">Leia as propriedades e as relações do objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="5e062-107">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e062-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e062-108">Prerequisites</span></span>
<span data-ttu-id="5e062-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e062-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e062-111">Permission type</span></span>|<span data-ttu-id="5e062-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e062-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e062-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e062-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e062-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e062-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e062-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e062-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e062-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e062-116">Not supported.</span></span>|
|<span data-ttu-id="5e062-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e062-117">Application</span></span>|<span data-ttu-id="5e062-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e062-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e062-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e062-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e062-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5e062-120">Optional query parameters</span></span>
<span data-ttu-id="5e062-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5e062-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e062-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e062-122">Request headers</span></span>
|<span data-ttu-id="5e062-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e062-123">Header</span></span>|<span data-ttu-id="5e062-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5e062-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e062-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e062-125">Authorization</span></span>|<span data-ttu-id="5e062-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e062-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e062-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e062-127">Accept</span></span>|<span data-ttu-id="5e062-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5e062-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e062-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e062-129">Request body</span></span>
<span data-ttu-id="5e062-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e062-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e062-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e062-131">Response</span></span>
<span data-ttu-id="5e062-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e062-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e062-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e062-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e062-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e062-134">Request</span></span>
<span data-ttu-id="5e062-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e062-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="5e062-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e062-136">Response</span></span>
<span data-ttu-id="5e062-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e062-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 432

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
    "id": "886f167b-167b-886f-7b16-6f887b166f88",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



