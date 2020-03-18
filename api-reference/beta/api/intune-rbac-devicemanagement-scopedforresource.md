---
title: função scopedForResource
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21b683f56c39bcb7bdd62354a504992a197065af
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801730"
---
# <a name="scopedforresource-function"></a><span data-ttu-id="5214f-103">função scopedForResource</span><span class="sxs-lookup"><span data-stu-id="5214f-103">scopedForResource function</span></span>

> <span data-ttu-id="5214f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5214f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5214f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5214f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5214f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5214f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5214f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5214f-107">Prerequisites</span></span>
<span data-ttu-id="5214f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5214f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5214f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5214f-110">Permission type</span></span>|<span data-ttu-id="5214f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5214f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5214f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5214f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5214f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5214f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5214f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5214f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5214f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5214f-115">Not supported.</span></span>|
|<span data-ttu-id="5214f-116">Application</span><span class="sxs-lookup"><span data-stu-id="5214f-116">Application</span></span>|<span data-ttu-id="5214f-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5214f-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5214f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5214f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/scopedForResource
```

## <a name="request-headers"></a><span data-ttu-id="5214f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5214f-119">Request headers</span></span>
|<span data-ttu-id="5214f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5214f-120">Header</span></span>|<span data-ttu-id="5214f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5214f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5214f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5214f-122">Authorization</span></span>|<span data-ttu-id="5214f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5214f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5214f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5214f-124">Accept</span></span>|<span data-ttu-id="5214f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5214f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5214f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5214f-126">Request body</span></span>
<span data-ttu-id="5214f-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="5214f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5214f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="5214f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5214f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5214f-129">Property</span></span>|<span data-ttu-id="5214f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5214f-130">Type</span></span>|<span data-ttu-id="5214f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5214f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5214f-132">recurso</span><span class="sxs-lookup"><span data-stu-id="5214f-132">resource</span></span>|<span data-ttu-id="5214f-133">String</span><span class="sxs-lookup"><span data-stu-id="5214f-133">String</span></span>|<span data-ttu-id="5214f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5214f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5214f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5214f-135">Response</span></span>
<span data-ttu-id="5214f-136">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5214f-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5214f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5214f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5214f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5214f-138">Request</span></span>
<span data-ttu-id="5214f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5214f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/scopedForResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5214f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5214f-140">Response</span></span>
<span data-ttu-id="5214f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5214f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




