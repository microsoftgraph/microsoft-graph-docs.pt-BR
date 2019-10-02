---
title: Obter telecomExpenseManagementPartner
description: Ler propriedades de leitura e relações do objeto telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af43f0615d15e067f8b6216a401a07b66f083217
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361168"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="5eb79-103">Obter telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="5eb79-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="5eb79-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5eb79-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eb79-105">Ler propriedades de leitura e relações do objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="5eb79-105">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5eb79-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5eb79-106">Prerequisites</span></span>
<span data-ttu-id="5eb79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eb79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eb79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5eb79-109">Permission type</span></span>|<span data-ttu-id="5eb79-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5eb79-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eb79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5eb79-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5eb79-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5eb79-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5eb79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5eb79-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eb79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5eb79-114">Not supported.</span></span>|
|<span data-ttu-id="5eb79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5eb79-115">Application</span></span>|<span data-ttu-id="5eb79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5eb79-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eb79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5eb79-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5eb79-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5eb79-118">Optional query parameters</span></span>
<span data-ttu-id="5eb79-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb79-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eb79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb79-120">Request headers</span></span>
|<span data-ttu-id="5eb79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5eb79-121">Header</span></span>|<span data-ttu-id="5eb79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5eb79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eb79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5eb79-123">Authorization</span></span>|<span data-ttu-id="5eb79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5eb79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eb79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5eb79-125">Accept</span></span>|<span data-ttu-id="5eb79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5eb79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eb79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb79-127">Request body</span></span>
<span data-ttu-id="5eb79-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5eb79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eb79-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb79-129">Response</span></span>
<span data-ttu-id="5eb79-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb79-130">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eb79-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5eb79-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5eb79-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb79-132">Request</span></span>
<span data-ttu-id="5eb79-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5eb79-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="5eb79-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb79-134">Response</span></span>
<span data-ttu-id="5eb79-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5eb79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```




