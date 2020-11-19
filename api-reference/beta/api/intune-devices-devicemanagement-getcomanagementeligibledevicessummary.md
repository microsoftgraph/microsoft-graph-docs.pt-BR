---
title: função getComanagementEligibleDevicesSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a023d7b01e6981cacec9929c208275dfb9795828
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49225682"
---
# <a name="getcomanagementeligibledevicessummary-function"></a><span data-ttu-id="08331-103">função getComanagementEligibleDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="08331-103">getComanagementEligibleDevicesSummary function</span></span>

<span data-ttu-id="08331-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08331-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08331-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08331-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08331-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08331-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08331-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="08331-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08331-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08331-108">Prerequisites</span></span>
<span data-ttu-id="08331-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08331-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08331-111">Permission type</span></span>|<span data-ttu-id="08331-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08331-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08331-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08331-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08331-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="08331-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="08331-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08331-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08331-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08331-116">Not supported.</span></span>|
|<span data-ttu-id="08331-117">Application</span><span class="sxs-lookup"><span data-stu-id="08331-117">Application</span></span>|<span data-ttu-id="08331-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="08331-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08331-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08331-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagementEligibleDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="08331-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08331-120">Request headers</span></span>
|<span data-ttu-id="08331-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08331-121">Header</span></span>|<span data-ttu-id="08331-122">Valor</span><span class="sxs-lookup"><span data-stu-id="08331-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08331-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08331-123">Authorization</span></span>|<span data-ttu-id="08331-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08331-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08331-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08331-125">Accept</span></span>|<span data-ttu-id="08331-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08331-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08331-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08331-127">Request body</span></span>
<span data-ttu-id="08331-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08331-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08331-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="08331-129">Response</span></span>
<span data-ttu-id="08331-130">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [comanagementEligibleDevicesSummary](../resources/intune-devices-comanagementeligibledevicessummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08331-130">If successful, this function returns a `200 OK` response code and a [comanagementEligibleDevicesSummary](../resources/intune-devices-comanagementeligibledevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08331-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08331-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="08331-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08331-132">Request</span></span>
<span data-ttu-id="08331-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08331-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagementEligibleDevicesSummary
```

### <a name="response"></a><span data-ttu-id="08331-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="08331-134">Response</span></span>
<span data-ttu-id="08331-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08331-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




