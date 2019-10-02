---
title: Acessar remoteAssistancePartner
description: Leia as propriedades e as relações do objeto remoteAssistancePartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6070c52c5b0df54f1f01c91c22d690e0111565bd
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361613"
---
# <a name="get-remoteassistancepartner"></a><span data-ttu-id="41cb2-103">Acessar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="41cb2-103">Get remoteAssistancePartner</span></span>

> <span data-ttu-id="41cb2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41cb2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41cb2-105">Leia as propriedades e as relações do objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="41cb2-105">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41cb2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41cb2-106">Prerequisites</span></span>
<span data-ttu-id="41cb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41cb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41cb2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41cb2-109">Permission type</span></span>|<span data-ttu-id="41cb2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41cb2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41cb2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41cb2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41cb2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="41cb2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="41cb2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41cb2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41cb2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41cb2-114">Not supported.</span></span>|
|<span data-ttu-id="41cb2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41cb2-115">Application</span></span>|<span data-ttu-id="41cb2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41cb2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41cb2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41cb2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41cb2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41cb2-118">Optional query parameters</span></span>
<span data-ttu-id="41cb2-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41cb2-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41cb2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41cb2-120">Request headers</span></span>
|<span data-ttu-id="41cb2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41cb2-121">Header</span></span>|<span data-ttu-id="41cb2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="41cb2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41cb2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41cb2-123">Authorization</span></span>|<span data-ttu-id="41cb2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41cb2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41cb2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41cb2-125">Accept</span></span>|<span data-ttu-id="41cb2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41cb2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41cb2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41cb2-127">Request body</span></span>
<span data-ttu-id="41cb2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41cb2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41cb2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="41cb2-129">Response</span></span>
<span data-ttu-id="41cb2-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41cb2-130">If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41cb2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41cb2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="41cb2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41cb2-132">Request</span></span>
<span data-ttu-id="41cb2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41cb2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="41cb2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="41cb2-134">Response</span></span>
<span data-ttu-id="41cb2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41cb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteAssistancePartner",
    "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
    "displayName": "Display Name value",
    "onboardingUrl": "https://example.com/onboardingUrl/",
    "onboardingStatus": "onboarding",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```




