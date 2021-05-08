---
title: 'updatableAsset: enrollAssetsById'
description: Registrar recursos updatableAsset do mesmo tipo no gerenciamento de atualizações pelo serviço de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 127817e3623b86854f8c69812c385a25aee323f4
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241163"
---
# <a name="updatableasset-enrollassetsbyid"></a><span data-ttu-id="d9c0e-103">updatableAsset: enrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="d9c0e-103">updatableAsset: enrollAssetsById</span></span>
<span data-ttu-id="d9c0e-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d9c0e-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9c0e-105">Registrar [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) do mesmo tipo no gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-105">Enroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type in update management by the deployment service.</span></span>

<span data-ttu-id="d9c0e-106">Você também pode usar o método [enrollAssets](windowsupdates-updatableasset-enrollassets.md) para registrar ativos.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-106">You can also use the method [enrollAssets](windowsupdates-updatableasset-enrollassets.md) to enroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9c0e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9c0e-107">Permissions</span></span>
<span data-ttu-id="d9c0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9c0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9c0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9c0e-110">Permission type</span></span>|<span data-ttu-id="d9c0e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9c0e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9c0e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9c0e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9c0e-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9c0e-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="d9c0e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9c0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9c0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-115">Not supported.</span></span>|
|<span data-ttu-id="d9c0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9c0e-116">Application</span></span>|<span data-ttu-id="d9c0e-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9c0e-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9c0e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9c0e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/enrollAssetsById
```

## <a name="request-headers"></a><span data-ttu-id="d9c0e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c0e-119">Request headers</span></span>
|<span data-ttu-id="d9c0e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d9c0e-120">Name</span></span>|<span data-ttu-id="d9c0e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9c0e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9c0e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9c0e-122">Authorization</span></span>|<span data-ttu-id="d9c0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d9c0e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9c0e-125">Content-Type</span></span>|<span data-ttu-id="d9c0e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9c0e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c0e-128">Request body</span></span>
<span data-ttu-id="d9c0e-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d9c0e-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d9c0e-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d9c0e-131">Parameter</span></span>|<span data-ttu-id="d9c0e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9c0e-132">Type</span></span>|<span data-ttu-id="d9c0e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9c0e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9c0e-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="d9c0e-134">updateCategory</span></span>|<span data-ttu-id="d9c0e-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="d9c0e-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="d9c0e-136">A categoria de atualizações para o serviço gerenciar.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-136">The category of updates for the service to manage.</span></span> <span data-ttu-id="d9c0e-137">Oferece suporte a um subconjunto dos valores **para updateCategory**.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="d9c0e-138">Os valores possíveis são: `feature` .</span><span class="sxs-lookup"><span data-stu-id="d9c0e-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="d9c0e-139">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="d9c0e-139">memberEntityType</span></span>|<span data-ttu-id="d9c0e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9c0e-140">String</span></span>|<span data-ttu-id="d9c0e-141">O tipo completo dos **recursos updatableAsset.**</span><span class="sxs-lookup"><span data-stu-id="d9c0e-141">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="d9c0e-142">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="d9c0e-142">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|
|<span data-ttu-id="d9c0e-143">ids</span><span class="sxs-lookup"><span data-stu-id="d9c0e-143">ids</span></span>|<span data-ttu-id="d9c0e-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9c0e-144">String collection</span></span>|<span data-ttu-id="d9c0e-145">Lista de identificadores correspondentes aos **recursos updatableAsset** para se inscrever no gerenciamento de atualizações pelo serviço para **a atualização determinadaCategory**.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-145">List of identifiers corresponding to the **updatableAsset** resources to enroll in update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="d9c0e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c0e-146">Response</span></span>

<span data-ttu-id="d9c0e-147">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-147">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="d9c0e-148">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9c0e-148">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9c0e-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9c0e-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9c0e-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c0e-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d9c0e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9c0e-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableasset_enrollassetsbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssetsById
Content-Type: application/json

{
  "updateCategory": "feature",
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice",
  "ids": [
    "String",
    "String",
    "String"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d9c0e-152">C#</span><span class="sxs-lookup"><span data-stu-id="d9c0e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableasset-enrollassetsbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9c0e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9c0e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableasset-enrollassetsbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9c0e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9c0e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableasset-enrollassetsbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9c0e-155">Java</span><span class="sxs-lookup"><span data-stu-id="d9c0e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableasset-enrollassetsbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d9c0e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c0e-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

