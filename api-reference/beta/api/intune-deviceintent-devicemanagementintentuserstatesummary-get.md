---
title: Obter deviceManagementIntentUserStateSummary
description: Leia as propriedades e as relações do objeto deviceManagementIntentUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 045302184bdf29da4c70f96bc2b3257f10882739
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734410"
---
# <a name="get-devicemanagementintentuserstatesummary"></a><span data-ttu-id="c71d5-103">Obter deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="c71d5-103">Get deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="c71d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c71d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c71d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c71d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c71d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c71d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c71d5-107">Leia as propriedades e as relações do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c71d5-107">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c71d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c71d5-108">Prerequisites</span></span>
<span data-ttu-id="c71d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c71d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c71d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c71d5-111">Permission type</span></span>|<span data-ttu-id="c71d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c71d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c71d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c71d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c71d5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c71d5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c71d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c71d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c71d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c71d5-116">Not supported.</span></span>|
|<span data-ttu-id="c71d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c71d5-117">Application</span></span>|<span data-ttu-id="c71d5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c71d5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c71d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c71d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c71d5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c71d5-120">Optional query parameters</span></span>
<span data-ttu-id="c71d5-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c71d5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c71d5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c71d5-122">Request headers</span></span>
|<span data-ttu-id="c71d5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c71d5-123">Header</span></span>|<span data-ttu-id="c71d5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c71d5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c71d5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c71d5-125">Authorization</span></span>|<span data-ttu-id="c71d5-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c71d5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c71d5-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c71d5-127">Accept</span></span>|<span data-ttu-id="c71d5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c71d5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c71d5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c71d5-129">Request body</span></span>
<span data-ttu-id="c71d5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c71d5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c71d5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c71d5-131">Response</span></span>
<span data-ttu-id="c71d5-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c71d5-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c71d5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c71d5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c71d5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c71d5-134">Request</span></span>
<span data-ttu-id="c71d5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c71d5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="c71d5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c71d5-136">Response</span></span>
<span data-ttu-id="c71d5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c71d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





