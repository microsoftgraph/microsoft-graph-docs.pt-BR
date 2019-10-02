---
title: Obter vppToken
description: Ler propriedades e relações de objetos vppToken.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 368a858879510c855eeec6b64049eb44d50824a9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362110"
---
# <a name="get-vpptoken"></a><span data-ttu-id="45d00-103">Obter vppToken</span><span class="sxs-lookup"><span data-stu-id="45d00-103">Get vppToken</span></span>

> <span data-ttu-id="45d00-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45d00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d00-105">Ler propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="45d00-105">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45d00-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45d00-106">Prerequisites</span></span>
<span data-ttu-id="45d00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45d00-109">Permission type</span></span>|<span data-ttu-id="45d00-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45d00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45d00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45d00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45d00-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="45d00-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="45d00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45d00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45d00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45d00-114">Not supported.</span></span>|
|<span data-ttu-id="45d00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45d00-115">Application</span></span>|<span data-ttu-id="45d00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45d00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45d00-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45d00-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45d00-118">Optional query parameters</span></span>
<span data-ttu-id="45d00-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45d00-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45d00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45d00-120">Request headers</span></span>
|<span data-ttu-id="45d00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45d00-121">Header</span></span>|<span data-ttu-id="45d00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45d00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45d00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45d00-123">Authorization</span></span>|<span data-ttu-id="45d00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45d00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45d00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45d00-125">Accept</span></span>|<span data-ttu-id="45d00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45d00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45d00-127">Request body</span></span>
<span data-ttu-id="45d00-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45d00-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45d00-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="45d00-129">Response</span></span>
<span data-ttu-id="45d00-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45d00-130">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d00-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45d00-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45d00-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45d00-132">Request</span></span>
<span data-ttu-id="45d00-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45d00-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="45d00-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="45d00-134">Response</span></span>
<span data-ttu-id="45d00-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45d00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




