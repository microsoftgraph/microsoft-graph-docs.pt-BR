---
title: Obter vppToken
description: Ler propriedades e relações de objetos vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7e97b6e7a304142b2d9646ff90232e35c077f98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997372"
---
# <a name="get-vpptoken"></a><span data-ttu-id="d0689-103">Obter vppToken</span><span class="sxs-lookup"><span data-stu-id="d0689-103">Get vppToken</span></span>

<span data-ttu-id="d0689-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0689-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0689-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0689-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0689-106">Ler propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="d0689-106">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0689-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0689-107">Prerequisites</span></span>
<span data-ttu-id="d0689-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0689-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0689-110">Permission type</span></span>|<span data-ttu-id="d0689-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0689-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0689-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0689-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0689-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0689-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d0689-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0689-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0689-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0689-115">Not supported.</span></span>|
|<span data-ttu-id="d0689-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0689-116">Application</span></span>|<span data-ttu-id="d0689-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0689-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0689-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0689-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0689-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0689-119">Optional query parameters</span></span>
<span data-ttu-id="d0689-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0689-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0689-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0689-121">Request headers</span></span>
|<span data-ttu-id="d0689-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0689-122">Header</span></span>|<span data-ttu-id="d0689-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d0689-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0689-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0689-124">Authorization</span></span>|<span data-ttu-id="d0689-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0689-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0689-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0689-126">Accept</span></span>|<span data-ttu-id="d0689-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d0689-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0689-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0689-128">Request body</span></span>
<span data-ttu-id="d0689-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0689-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0689-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0689-130">Response</span></span>
<span data-ttu-id="d0689-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0689-131">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0689-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0689-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0689-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0689-133">Request</span></span>
<span data-ttu-id="d0689-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0689-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="d0689-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0689-135">Response</span></span>
<span data-ttu-id="d0689-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0689-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```









