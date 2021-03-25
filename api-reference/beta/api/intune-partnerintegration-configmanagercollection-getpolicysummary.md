---
title: função getPolicySummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1421d45155a841202ba3c13e3c7eabd12b6a0013
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156804"
---
# <a name="getpolicysummary-function"></a><span data-ttu-id="3862a-103">função getPolicySummary</span><span class="sxs-lookup"><span data-stu-id="3862a-103">getPolicySummary function</span></span>

<span data-ttu-id="3862a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3862a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3862a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3862a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3862a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3862a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3862a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3862a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3862a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3862a-108">Prerequisites</span></span>
<span data-ttu-id="3862a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3862a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3862a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3862a-111">Permission type</span></span>|<span data-ttu-id="3862a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3862a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3862a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3862a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3862a-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3862a-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3862a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3862a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3862a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3862a-116">Not supported.</span></span>|
|<span data-ttu-id="3862a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3862a-117">Application</span></span>|<span data-ttu-id="3862a-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3862a-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3862a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3862a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configManagerCollections/getPolicySummary
```

## <a name="request-headers"></a><span data-ttu-id="3862a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3862a-120">Request headers</span></span>
|<span data-ttu-id="3862a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3862a-121">Header</span></span>|<span data-ttu-id="3862a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3862a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3862a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3862a-123">Authorization</span></span>|<span data-ttu-id="3862a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3862a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3862a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3862a-125">Accept</span></span>|<span data-ttu-id="3862a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3862a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3862a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3862a-127">Request body</span></span>
<span data-ttu-id="3862a-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="3862a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3862a-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="3862a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3862a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3862a-130">Property</span></span>|<span data-ttu-id="3862a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3862a-131">Type</span></span>|<span data-ttu-id="3862a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3862a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3862a-133">policyId</span><span class="sxs-lookup"><span data-stu-id="3862a-133">policyId</span></span>|<span data-ttu-id="3862a-134">String</span><span class="sxs-lookup"><span data-stu-id="3862a-134">String</span></span>|<span data-ttu-id="3862a-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3862a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3862a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3862a-136">Response</span></span>
<span data-ttu-id="3862a-137">Se tiver êxito, essa função retornará um código `200 OK` de resposta e um [configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3862a-137">If successful, this function returns a `200 OK` response code and a [configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3862a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3862a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3862a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3862a-139">Request</span></span>
<span data-ttu-id="3862a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3862a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configManagerCollections/getPolicySummary(policyId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="3862a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3862a-141">Response</span></span>
<span data-ttu-id="3862a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3862a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "value": {
    "@odata.type": "microsoft.graph.configManagerPolicySummary",
    "targetedDeviceCount": 3,
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "failedDeviceCount": 1,
    "pendingDeviceCount": 2,
    "enforcedDeviceCount": 3
  }
}
```




