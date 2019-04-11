---
title: Obter securityBaselineStateSummary
description: Leia as propriedades e as relações do objeto securityBaselineStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1539772b4a0a270dcae1d05af67133f257ff866b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804813"
---
# <a name="get-securitybaselinestatesummary"></a><span data-ttu-id="c1ccd-103">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="c1ccd-103">Get securityBaselineStateSummary</span></span>

> <span data-ttu-id="c1ccd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1ccd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ccd-106">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c1ccd-106">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1ccd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1ccd-107">Prerequisites</span></span>
<span data-ttu-id="c1ccd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ccd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1ccd-110">Permission type</span></span>|<span data-ttu-id="c1ccd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1ccd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1ccd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1ccd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1ccd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1ccd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c1ccd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1ccd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ccd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-115">Not supported.</span></span>|
|<span data-ttu-id="c1ccd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1ccd-116">Application</span></span>|<span data-ttu-id="c1ccd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ccd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1ccd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1ccd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1ccd-119">Optional query parameters</span></span>
<span data-ttu-id="c1ccd-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1ccd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ccd-121">Request headers</span></span>
|<span data-ttu-id="c1ccd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1ccd-122">Header</span></span>|<span data-ttu-id="c1ccd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c1ccd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1ccd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1ccd-124">Authorization</span></span>|<span data-ttu-id="c1ccd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1ccd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1ccd-126">Accept</span></span>|<span data-ttu-id="c1ccd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ccd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ccd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ccd-128">Request body</span></span>
<span data-ttu-id="c1ccd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1ccd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ccd-130">Response</span></span>
<span data-ttu-id="c1ccd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-131">If successful, this method returns a `200 OK` response code and [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ccd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1ccd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1ccd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ccd-133">Request</span></span>
<span data-ttu-id="c1ccd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

### <a name="response"></a><span data-ttu-id="c1ccd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ccd-135">Response</span></span>
<span data-ttu-id="c1ccd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1ccd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





