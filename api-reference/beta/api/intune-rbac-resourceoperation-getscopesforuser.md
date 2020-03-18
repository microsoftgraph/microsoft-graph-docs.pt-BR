---
title: função Getscopesforuser à
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aeb1ce22db3f60cb375609e74dc567708b422fc4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801702"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="51462-103">função Getscopesforuser à</span><span class="sxs-lookup"><span data-stu-id="51462-103">getScopesForUser function</span></span>

> <span data-ttu-id="51462-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51462-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51462-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51462-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51462-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51462-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51462-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51462-107">Prerequisites</span></span>
<span data-ttu-id="51462-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51462-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51462-110">Permission type</span></span>|<span data-ttu-id="51462-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51462-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51462-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51462-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51462-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="51462-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="51462-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51462-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51462-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51462-115">Not supported.</span></span>|
|<span data-ttu-id="51462-116">Application</span><span class="sxs-lookup"><span data-stu-id="51462-116">Application</span></span>|<span data-ttu-id="51462-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="51462-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51462-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51462-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="51462-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51462-119">Request headers</span></span>
|<span data-ttu-id="51462-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51462-120">Header</span></span>|<span data-ttu-id="51462-121">Valor</span><span class="sxs-lookup"><span data-stu-id="51462-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51462-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="51462-122">Authorization</span></span>|<span data-ttu-id="51462-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51462-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51462-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51462-124">Accept</span></span>|<span data-ttu-id="51462-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51462-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51462-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51462-126">Request body</span></span>
<span data-ttu-id="51462-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="51462-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="51462-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="51462-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="51462-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51462-129">Property</span></span>|<span data-ttu-id="51462-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="51462-130">Type</span></span>|<span data-ttu-id="51462-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="51462-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51462-132">ID</span><span class="sxs-lookup"><span data-stu-id="51462-132">userid</span></span>|<span data-ttu-id="51462-133">String</span><span class="sxs-lookup"><span data-stu-id="51462-133">String</span></span>|<span data-ttu-id="51462-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51462-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="51462-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="51462-135">Response</span></span>
<span data-ttu-id="51462-136">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51462-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51462-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51462-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="51462-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51462-138">Request</span></span>
<span data-ttu-id="51462-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51462-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="51462-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="51462-140">Response</span></span>
<span data-ttu-id="51462-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51462-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




