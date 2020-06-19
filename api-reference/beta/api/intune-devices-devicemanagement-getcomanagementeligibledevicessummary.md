---
title: função getComanagementEligibleDevicesSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 097a6ef17a1d08cb8342cfa13f6a474dcb13ad86
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792370"
---
# <a name="getcomanagementeligibledevicessummary-function"></a><span data-ttu-id="1c70e-103">função getComanagementEligibleDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="1c70e-103">getComanagementEligibleDevicesSummary function</span></span>

<span data-ttu-id="1c70e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c70e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c70e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c70e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c70e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c70e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c70e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c70e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c70e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c70e-108">Prerequisites</span></span>
<span data-ttu-id="1c70e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1c70e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1c70e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c70e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c70e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c70e-111">Permission type</span></span>|<span data-ttu-id="1c70e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c70e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c70e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c70e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c70e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c70e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1c70e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c70e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c70e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c70e-116">Not supported.</span></span>|
|<span data-ttu-id="1c70e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c70e-117">Application</span></span>|<span data-ttu-id="1c70e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c70e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c70e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c70e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagementEligibleDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="1c70e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c70e-120">Request headers</span></span>
|<span data-ttu-id="1c70e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c70e-121">Header</span></span>|<span data-ttu-id="1c70e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c70e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c70e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c70e-123">Authorization</span></span>|<span data-ttu-id="1c70e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c70e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c70e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c70e-125">Accept</span></span>|<span data-ttu-id="1c70e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c70e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c70e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c70e-127">Request body</span></span>
<span data-ttu-id="1c70e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c70e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c70e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c70e-129">Response</span></span>
<span data-ttu-id="1c70e-130">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [comanagementEligibleDevicesSummary](../resources/intune-devices-comanagementeligibledevicessummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c70e-130">If successful, this function returns a `200 OK` response code and a [comanagementEligibleDevicesSummary](../resources/intune-devices-comanagementeligibledevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c70e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c70e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c70e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c70e-132">Request</span></span>
<span data-ttu-id="1c70e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c70e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagementEligibleDevicesSummary
```

### <a name="response"></a><span data-ttu-id="1c70e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c70e-134">Response</span></span>
<span data-ttu-id="1c70e-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1c70e-135">Here is an example of the response.</span></span> <span data-ttu-id="1c70e-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1c70e-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1c70e-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1c70e-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary",
    "comanagedCount": 14,
    "eligibleCount": 13,
    "eligibleButNotAzureAdJoinedCount": 0,
    "needsOsUpdateCount": 2,
    "ineligibleCount": 15
  }
}
```



