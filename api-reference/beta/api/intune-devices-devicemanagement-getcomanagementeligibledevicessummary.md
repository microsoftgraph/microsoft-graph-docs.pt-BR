---
title: função getComanagementEligibleDevicesSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6db71f378c771f09160c3534b947ec71510158d6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146248"
---
# <a name="getcomanagementeligibledevicessummary-function"></a><span data-ttu-id="1d7cd-103">função getComanagementEligibleDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="1d7cd-103">getComanagementEligibleDevicesSummary function</span></span>

<span data-ttu-id="1d7cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d7cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d7cd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d7cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d7cd-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1d7cd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d7cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d7cd-108">Prerequisites</span></span>
<span data-ttu-id="1d7cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d7cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d7cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d7cd-111">Permission type</span></span>|<span data-ttu-id="1d7cd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d7cd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d7cd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d7cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d7cd-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7cd-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1d7cd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d7cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d7cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-116">Not supported.</span></span>|
|<span data-ttu-id="1d7cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d7cd-117">Application</span></span>|<span data-ttu-id="1d7cd-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7cd-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d7cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d7cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagementEligibleDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="1d7cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7cd-120">Request headers</span></span>
|<span data-ttu-id="1d7cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d7cd-121">Header</span></span>|<span data-ttu-id="1d7cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1d7cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d7cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d7cd-123">Authorization</span></span>|<span data-ttu-id="1d7cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d7cd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d7cd-125">Accept</span></span>|<span data-ttu-id="1d7cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d7cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d7cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7cd-127">Request body</span></span>
<span data-ttu-id="1d7cd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d7cd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d7cd-129">Response</span></span>
<span data-ttu-id="1d7cd-130">Se tiver êxito, essa função retornará um código de resposta e um `200 OK` [comanagementEligibleDevicesSummary](../resources/intune-devices-comanagementeligibledevicessummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-130">If successful, this function returns a `200 OK` response code and a [comanagementEligibleDevicesSummary](../resources/intune-devices-comanagementeligibledevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d7cd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d7cd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d7cd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d7cd-132">Request</span></span>
<span data-ttu-id="1d7cd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagementEligibleDevicesSummary
```

### <a name="response"></a><span data-ttu-id="1d7cd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d7cd-134">Response</span></span>
<span data-ttu-id="1d7cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d7cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




