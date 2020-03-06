---
title: Obter telecomExpenseManagementPartner
description: Ler propriedades de leitura e relações do objeto telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ed83eeb2552ac8f0811f25765097807cf615e16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511919"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="15767-103">Obter telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="15767-103">Get telecomExpenseManagementPartner</span></span>

<span data-ttu-id="15767-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15767-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15767-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15767-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15767-106">Ler propriedades de leitura e relações do objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="15767-106">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15767-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15767-107">Prerequisites</span></span>
<span data-ttu-id="15767-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15767-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15767-110">Permission type</span></span>|<span data-ttu-id="15767-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15767-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15767-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15767-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15767-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15767-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="15767-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15767-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15767-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15767-115">Not supported.</span></span>|
|<span data-ttu-id="15767-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15767-116">Application</span></span>|<span data-ttu-id="15767-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15767-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15767-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15767-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15767-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15767-119">Optional query parameters</span></span>
<span data-ttu-id="15767-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="15767-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15767-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15767-121">Request headers</span></span>
|<span data-ttu-id="15767-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15767-122">Header</span></span>|<span data-ttu-id="15767-123">Valor</span><span class="sxs-lookup"><span data-stu-id="15767-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15767-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15767-124">Authorization</span></span>|<span data-ttu-id="15767-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15767-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15767-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15767-126">Accept</span></span>|<span data-ttu-id="15767-127">application/json</span><span class="sxs-lookup"><span data-stu-id="15767-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15767-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15767-128">Request body</span></span>
<span data-ttu-id="15767-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15767-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15767-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="15767-130">Response</span></span>
<span data-ttu-id="15767-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15767-131">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15767-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15767-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="15767-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15767-133">Request</span></span>
<span data-ttu-id="15767-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15767-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="15767-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="15767-135">Response</span></span>
<span data-ttu-id="15767-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15767-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




