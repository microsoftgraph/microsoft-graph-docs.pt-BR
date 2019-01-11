---
title: Obter telecomExpenseManagementPartner
description: Ler propriedades de leitura e relações do objeto telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba9e9933424bd63277ecc80acf3d3aaecdd7e4ee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818155"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="1e740-103">Obter telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1e740-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="1e740-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e740-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e740-105">Ler propriedades de leitura e relações do objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="1e740-105">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e740-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e740-106">Prerequisites</span></span>
<span data-ttu-id="1e740-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e740-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e740-109">Permission type</span></span>|<span data-ttu-id="1e740-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e740-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e740-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e740-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e740-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e740-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1e740-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e740-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e740-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e740-114">Not supported.</span></span>|
|<span data-ttu-id="1e740-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e740-115">Application</span></span>|<span data-ttu-id="1e740-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e740-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e740-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e740-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e740-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1e740-118">Optional query parameters</span></span>
<span data-ttu-id="1e740-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e740-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1e740-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e740-120">Request headers</span></span>
|<span data-ttu-id="1e740-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e740-121">Header</span></span>|<span data-ttu-id="1e740-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e740-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e740-123">Authorization</span></span>|<span data-ttu-id="1e740-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e740-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e740-125">Accept</span></span>|<span data-ttu-id="1e740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e740-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e740-127">Request body</span></span>
<span data-ttu-id="1e740-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e740-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e740-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e740-129">Response</span></span>
<span data-ttu-id="1e740-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e740-130">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e740-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e740-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e740-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e740-132">Request</span></span>
<span data-ttu-id="1e740-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e740-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="1e740-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e740-134">Response</span></span>
<span data-ttu-id="1e740-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e740-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



