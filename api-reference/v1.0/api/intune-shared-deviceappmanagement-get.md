---
title: Get deviceAppManagement
description: Ler propriedades e relações de objetos de deviceAppManagement.
author: tfitzmac
ms.openlocfilehash: 269e749c7fae0b2eeb397d86907a7cf2d6653ee7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314193"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="4695f-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="4695f-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="4695f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4695f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4695f-105">Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4695f-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4695f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4695f-106">Prerequisites</span></span>

<span data-ttu-id="4695f-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4695f-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4695f-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4695f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="4695f-109">Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4695f-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="4695f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4695f-110">Permission type</span></span>|<span data-ttu-id="4695f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4695f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4695f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4695f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4695f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4695f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="4695f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4695f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4695f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4695f-115">Not supported.</span></span>|
|<span data-ttu-id="4695f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4695f-116">Application</span></span>|<span data-ttu-id="4695f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4695f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4695f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4695f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4695f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4695f-119">Optional query parameters</span></span>
<span data-ttu-id="4695f-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4695f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4695f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4695f-121">Request headers</span></span>
|<span data-ttu-id="4695f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4695f-122">Header</span></span>|<span data-ttu-id="4695f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4695f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4695f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4695f-124">Authorization</span></span>|<span data-ttu-id="4695f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4695f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4695f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4695f-126">Accept</span></span>|<span data-ttu-id="4695f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4695f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4695f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4695f-128">Request body</span></span>
<span data-ttu-id="4695f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4695f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4695f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4695f-130">Response</span></span>
<span data-ttu-id="4695f-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4695f-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="4695f-132">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="4695f-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="4695f-133">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="4695f-133">Example response</span></span>
<span data-ttu-id="4695f-134">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="4695f-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4695f-135">Serão retornadas todas as propriedades de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4695f-135">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



