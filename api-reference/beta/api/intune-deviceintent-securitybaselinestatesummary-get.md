---
title: Obter securityBaselineStateSummary
description: Leia as propriedades e as relações do objeto securityBaselineStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4375a535bf7389c1a36eafbd1ad10a0f3fb84da
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814859"
---
# <a name="get-securitybaselinestatesummary"></a><span data-ttu-id="d1d14-103">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d1d14-103">Get securityBaselineStateSummary</span></span>

> <span data-ttu-id="d1d14-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1d14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1d14-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1d14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1d14-106">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d1d14-106">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1d14-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1d14-107">Prerequisites</span></span>
<span data-ttu-id="d1d14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1d14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1d14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1d14-110">Permission type</span></span>|<span data-ttu-id="d1d14-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1d14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1d14-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1d14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1d14-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1d14-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d1d14-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1d14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1d14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1d14-115">Not supported.</span></span>|
|<span data-ttu-id="d1d14-116">Application</span><span class="sxs-lookup"><span data-stu-id="d1d14-116">Application</span></span>|<span data-ttu-id="d1d14-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1d14-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1d14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1d14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1d14-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1d14-119">Optional query parameters</span></span>
<span data-ttu-id="d1d14-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d14-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1d14-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d14-121">Request headers</span></span>
|<span data-ttu-id="d1d14-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1d14-122">Header</span></span>|<span data-ttu-id="d1d14-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d1d14-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1d14-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1d14-124">Authorization</span></span>|<span data-ttu-id="d1d14-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1d14-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1d14-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1d14-126">Accept</span></span>|<span data-ttu-id="d1d14-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d1d14-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1d14-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d14-128">Request body</span></span>
<span data-ttu-id="d1d14-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1d14-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1d14-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d14-130">Response</span></span>
<span data-ttu-id="d1d14-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d14-131">If successful, this method returns a `200 OK` response code and [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1d14-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1d14-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1d14-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d14-133">Request</span></span>
<span data-ttu-id="d1d14-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1d14-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

### <a name="response"></a><span data-ttu-id="d1d14-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d14-135">Response</span></span>
<span data-ttu-id="d1d14-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1d14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
    "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
    "secureCount": 11,
    "notSecureCount": 14,
    "unknownCount": 12,
    "errorCount": 10,
    "conflictCount": 13,
    "notApplicableCount": 2
  }
}
```




