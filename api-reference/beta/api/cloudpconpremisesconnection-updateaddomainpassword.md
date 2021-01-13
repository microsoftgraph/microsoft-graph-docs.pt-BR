---
title: 'cloudPcOnPremisesConnection: updateAdDomainPassword'
description: Atualize a senha do domínio do AD para um onPremisesConnection bem-sucedido.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ca47884a99b0feec3721708b7c16cbc426e53e90
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49845102"
---
# <a name="cloudpconpremisesconnection-updateaddomainpassword"></a><span data-ttu-id="d0fb6-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="d0fb6-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span></span>
<span data-ttu-id="d0fb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0fb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0fb6-105">Atualize a senha de domínio do Active Directory para [um onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="d0fb6-105">Update Active Directory domain password for an [onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="d0fb6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d0fb6-106">Permissions</span></span>
<span data-ttu-id="d0fb6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0fb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0fb6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0fb6-109">Permission type</span></span>|<span data-ttu-id="d0fb6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0fb6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0fb6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0fb6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0fb6-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0fb6-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d0fb6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0fb6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0fb6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-114">Not supported.</span></span>|
|<span data-ttu-id="d0fb6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0fb6-115">Application</span></span>|<span data-ttu-id="d0fb6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0fb6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0fb6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
```

## <a name="request-headers"></a><span data-ttu-id="d0fb6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0fb6-118">Request headers</span></span>
|<span data-ttu-id="d0fb6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d0fb6-119">Name</span></span>|<span data-ttu-id="d0fb6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0fb6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d0fb6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0fb6-121">Authorization</span></span>|<span data-ttu-id="d0fb6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0fb6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0fb6-124">Content-Type</span></span>|<span data-ttu-id="d0fb6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0fb6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0fb6-127">Request body</span></span>
<span data-ttu-id="d0fb6-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d0fb6-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d0fb6-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d0fb6-130">Parameter</span></span>|<span data-ttu-id="d0fb6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0fb6-131">Type</span></span>|<span data-ttu-id="d0fb6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0fb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0fb6-133">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="d0fb6-133">adDomainPassword</span></span>|<span data-ttu-id="d0fb6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0fb6-134">String</span></span>|<span data-ttu-id="d0fb6-135">A senha associada a adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="d0fb6-135">The password associated with adDomainUsername</span></span>|



## <a name="response"></a><span data-ttu-id="d0fb6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0fb6-136">Response</span></span>

<span data-ttu-id="d0fb6-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d0fb6-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0fb6-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0fb6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0fb6-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_updateaddomainpassword"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
Content-Type: application/json
Content-length: 36

{
  "adDomainPassword": "AdDomainPassword value"
}
```


### <a name="response"></a><span data-ttu-id="d0fb6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0fb6-140">Response</span></span>
<span data-ttu-id="d0fb6-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d0fb6-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
