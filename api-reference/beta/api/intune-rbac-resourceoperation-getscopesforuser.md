---
title: função Getscopesforuser à
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39d7899d5f95ce8808ce4f1dc978aa3a0115bee8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161842"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="5f96b-103">função Getscopesforuser à</span><span class="sxs-lookup"><span data-stu-id="5f96b-103">getScopesForUser function</span></span>

> <span data-ttu-id="5f96b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f96b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f96b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f96b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f96b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5f96b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f96b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f96b-107">Prerequisites</span></span>
<span data-ttu-id="5f96b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f96b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f96b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f96b-110">Permission type</span></span>|<span data-ttu-id="5f96b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f96b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f96b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f96b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f96b-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f96b-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5f96b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f96b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f96b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f96b-115">Not supported.</span></span>|
|<span data-ttu-id="5f96b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f96b-116">Application</span></span>|<span data-ttu-id="5f96b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f96b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f96b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f96b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="5f96b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f96b-119">Request headers</span></span>
|<span data-ttu-id="5f96b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f96b-120">Header</span></span>|<span data-ttu-id="5f96b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5f96b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f96b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f96b-122">Authorization</span></span>|<span data-ttu-id="5f96b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f96b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f96b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f96b-124">Accept</span></span>|<span data-ttu-id="5f96b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f96b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f96b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f96b-126">Request body</span></span>
<span data-ttu-id="5f96b-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="5f96b-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5f96b-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="5f96b-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5f96b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f96b-129">Property</span></span>|<span data-ttu-id="5f96b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f96b-130">Type</span></span>|<span data-ttu-id="5f96b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f96b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f96b-132">ID</span><span class="sxs-lookup"><span data-stu-id="5f96b-132">userid</span></span>|<span data-ttu-id="5f96b-133">String</span><span class="sxs-lookup"><span data-stu-id="5f96b-133">String</span></span>|<span data-ttu-id="5f96b-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5f96b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5f96b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f96b-135">Response</span></span>
<span data-ttu-id="5f96b-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f96b-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f96b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f96b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f96b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f96b-138">Request</span></span>
<span data-ttu-id="5f96b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f96b-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5f96b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f96b-140">Response</span></span>
<span data-ttu-id="5f96b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f96b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": [
    "Get Scopes For User value"
  ]
}
```




