---
title: Obter deviceManagementIntentUserStateSummary
description: Leia as propriedades e as relações do objeto deviceManagementIntentUserStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8abd7e067744669bfc78a47281297176e78d11a1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815146"
---
# <a name="get-devicemanagementintentuserstatesummary"></a><span data-ttu-id="d4793-103">Obter deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="d4793-103">Get deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="d4793-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4793-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4793-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4793-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4793-106">Leia as propriedades e as relações do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d4793-106">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4793-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4793-107">Prerequisites</span></span>
<span data-ttu-id="d4793-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4793-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4793-110">Permission type</span></span>|<span data-ttu-id="d4793-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4793-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4793-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4793-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4793-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4793-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d4793-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4793-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4793-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4793-115">Not supported.</span></span>|
|<span data-ttu-id="d4793-116">Application</span><span class="sxs-lookup"><span data-stu-id="d4793-116">Application</span></span>|<span data-ttu-id="d4793-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4793-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4793-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4793-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4793-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4793-119">Optional query parameters</span></span>
<span data-ttu-id="d4793-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4793-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4793-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4793-121">Request headers</span></span>
|<span data-ttu-id="d4793-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4793-122">Header</span></span>|<span data-ttu-id="d4793-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d4793-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4793-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4793-124">Authorization</span></span>|<span data-ttu-id="d4793-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4793-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4793-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4793-126">Accept</span></span>|<span data-ttu-id="d4793-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d4793-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4793-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4793-128">Request body</span></span>
<span data-ttu-id="d4793-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4793-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4793-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4793-130">Response</span></span>
<span data-ttu-id="d4793-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4793-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4793-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4793-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4793-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4793-133">Request</span></span>
<span data-ttu-id="d4793-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4793-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="d4793-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4793-135">Response</span></span>
<span data-ttu-id="d4793-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4793-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
    "id": "be567e02-7e02-be56-027e-56be027e56be",
    "conflictCount": 13,
    "errorCount": 10,
    "failedCount": 11,
    "notApplicableCount": 2,
    "successCount": 12
  }
}
```




