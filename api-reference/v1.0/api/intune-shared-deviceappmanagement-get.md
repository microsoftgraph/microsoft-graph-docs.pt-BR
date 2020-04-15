---
title: Get deviceAppManagement
description: Ler propriedades e relações do objeto deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04c77b7b82220e456471fe4ddb5bbfe2955a9b0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465835"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="b68ce-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="b68ce-103">Get deviceAppManagement</span></span>

<span data-ttu-id="b68ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b68ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b68ce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b68ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b68ce-106">Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="b68ce-106">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b68ce-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b68ce-107">Prerequisites</span></span>

<span data-ttu-id="b68ce-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b68ce-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b68ce-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b68ce-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b68ce-110">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b68ce-110">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b68ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b68ce-111">Permission type</span></span>|<span data-ttu-id="b68ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b68ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b68ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b68ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b68ce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b68ce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="b68ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b68ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b68ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b68ce-116">Not supported.</span></span>|
|<span data-ttu-id="b68ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b68ce-117">Application</span></span>|<span data-ttu-id="b68ce-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b68ce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b68ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b68ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b68ce-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b68ce-120">Optional query parameters</span></span>
<span data-ttu-id="b68ce-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b68ce-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b68ce-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b68ce-122">Request headers</span></span>
|<span data-ttu-id="b68ce-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b68ce-123">Header</span></span>|<span data-ttu-id="b68ce-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b68ce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b68ce-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b68ce-125">Authorization</span></span>|<span data-ttu-id="b68ce-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b68ce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b68ce-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b68ce-127">Accept</span></span>|<span data-ttu-id="b68ce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b68ce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b68ce-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b68ce-129">Request body</span></span>
<span data-ttu-id="b68ce-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b68ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b68ce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b68ce-131">Response</span></span>
<span data-ttu-id="b68ce-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b68ce-132">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="b68ce-133">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="b68ce-133">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="b68ce-134">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="b68ce-134">Example response</span></span>
<span data-ttu-id="b68ce-135">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="b68ce-135">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b68ce-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b68ce-136">All properties will be returned from an actual call.</span></span>

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






