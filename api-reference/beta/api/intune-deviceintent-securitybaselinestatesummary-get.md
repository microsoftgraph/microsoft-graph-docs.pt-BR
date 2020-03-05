---
title: Obter securityBaselineStateSummary
description: Leia as propriedades e as relações do objeto securityBaselineStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff25c2a1b269ff383446d73b89fb9f81542fef94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470165"
---
# <a name="get-securitybaselinestatesummary"></a><span data-ttu-id="41d26-103">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="41d26-103">Get securityBaselineStateSummary</span></span>

<span data-ttu-id="41d26-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="41d26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41d26-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41d26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41d26-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41d26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41d26-107">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="41d26-107">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41d26-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41d26-108">Prerequisites</span></span>
<span data-ttu-id="41d26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d26-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41d26-111">Permission type</span></span>|<span data-ttu-id="41d26-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41d26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41d26-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41d26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41d26-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d26-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41d26-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41d26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41d26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41d26-116">Not supported.</span></span>|
|<span data-ttu-id="41d26-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41d26-117">Application</span></span>|<span data-ttu-id="41d26-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d26-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41d26-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41d26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41d26-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41d26-120">Optional query parameters</span></span>
<span data-ttu-id="41d26-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41d26-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41d26-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41d26-122">Request headers</span></span>
|<span data-ttu-id="41d26-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41d26-123">Header</span></span>|<span data-ttu-id="41d26-124">Valor</span><span class="sxs-lookup"><span data-stu-id="41d26-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41d26-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="41d26-125">Authorization</span></span>|<span data-ttu-id="41d26-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d26-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41d26-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41d26-127">Accept</span></span>|<span data-ttu-id="41d26-128">application/json</span><span class="sxs-lookup"><span data-stu-id="41d26-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41d26-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41d26-129">Request body</span></span>
<span data-ttu-id="41d26-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41d26-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41d26-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d26-131">Response</span></span>
<span data-ttu-id="41d26-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41d26-132">If successful, this method returns a `200 OK` response code and [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d26-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41d26-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="41d26-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41d26-134">Request</span></span>
<span data-ttu-id="41d26-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41d26-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

### <a name="response"></a><span data-ttu-id="41d26-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d26-136">Response</span></span>
<span data-ttu-id="41d26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41d26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





