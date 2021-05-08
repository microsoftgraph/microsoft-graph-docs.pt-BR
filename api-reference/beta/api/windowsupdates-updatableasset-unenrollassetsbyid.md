---
title: 'updatableAsset: unenrollAssetsById'
description: Unenroll updatableAsset resources of the same type from update management by the deployment service.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 72a3e97aee449953204225d40fee236126bddaa1
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240685"
---
# <a name="updatableasset-unenrollassetsbyid"></a><span data-ttu-id="28b89-103">updatableAsset: unenrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="28b89-103">updatableAsset: unenrollAssetsById</span></span>
<span data-ttu-id="28b89-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="28b89-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b89-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type from update management by the deployment service.</span><span class="sxs-lookup"><span data-stu-id="28b89-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type from update management by the deployment service.</span></span>

<span data-ttu-id="28b89-106">Você também pode usar o [método unenrollAssets](windowsupdates-updatableasset-unenrollassets.md) para desemrollar ativos.</span><span class="sxs-lookup"><span data-stu-id="28b89-106">You can also use the method [unenrollAssets](windowsupdates-updatableasset-unenrollassets.md) to unenroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="28b89-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="28b89-107">Permissions</span></span>
<span data-ttu-id="28b89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28b89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28b89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28b89-110">Permission type</span></span>|<span data-ttu-id="28b89-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28b89-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28b89-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28b89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28b89-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28b89-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="28b89-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28b89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28b89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28b89-115">Not supported.</span></span>|
|<span data-ttu-id="28b89-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28b89-116">Application</span></span>|<span data-ttu-id="28b89-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28b89-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28b89-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28b89-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/unenrollAssetsById
```

## <a name="request-headers"></a><span data-ttu-id="28b89-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28b89-119">Request headers</span></span>
|<span data-ttu-id="28b89-120">Nome</span><span class="sxs-lookup"><span data-stu-id="28b89-120">Name</span></span>|<span data-ttu-id="28b89-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b89-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="28b89-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="28b89-122">Authorization</span></span>|<span data-ttu-id="28b89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b89-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="28b89-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28b89-125">Content-Type</span></span>|<span data-ttu-id="28b89-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b89-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28b89-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28b89-128">Request body</span></span>
<span data-ttu-id="28b89-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="28b89-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="28b89-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="28b89-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="28b89-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="28b89-131">Parameter</span></span>|<span data-ttu-id="28b89-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b89-132">Type</span></span>|<span data-ttu-id="28b89-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b89-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b89-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="28b89-134">updateCategory</span></span>|<span data-ttu-id="28b89-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="28b89-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="28b89-136">A categoria de atualizações para o serviço parar de gerenciar.</span><span class="sxs-lookup"><span data-stu-id="28b89-136">The category of updates for the service to stop managing.</span></span> <span data-ttu-id="28b89-137">Oferece suporte a um subconjunto dos valores **para updateCategory**.</span><span class="sxs-lookup"><span data-stu-id="28b89-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="28b89-138">Os valores possíveis são: `feature` .</span><span class="sxs-lookup"><span data-stu-id="28b89-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="28b89-139">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="28b89-139">memberEntityType</span></span>|<span data-ttu-id="28b89-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b89-140">String</span></span>|<span data-ttu-id="28b89-141">O tipo completo dos **recursos updatableAsset.**</span><span class="sxs-lookup"><span data-stu-id="28b89-141">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="28b89-142">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="28b89-142">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|
|<span data-ttu-id="28b89-143">ids</span><span class="sxs-lookup"><span data-stu-id="28b89-143">ids</span></span>|<span data-ttu-id="28b89-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b89-144">String collection</span></span>|<span data-ttu-id="28b89-145">Lista de identificadores correspondentes aos recursos **updatableAsset** a ser desempaculado do gerenciamento de atualizações pelo serviço para a **atualização determinadaCategory**.</span><span class="sxs-lookup"><span data-stu-id="28b89-145">List of identifiers corresponding to the **updatableAsset** resources to unenroll from update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="28b89-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b89-146">Response</span></span>

<span data-ttu-id="28b89-147">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="28b89-147">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="28b89-148">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28b89-148">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28b89-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28b89-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28b89-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b89-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="28b89-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="28b89-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassetsbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssetsById
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
# <a name="c"></a>[<span data-ttu-id="28b89-152">C#</span><span class="sxs-lookup"><span data-stu-id="28b89-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableasset-unenrollassetsbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28b89-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28b89-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableasset-unenrollassetsbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28b89-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28b89-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableasset-unenrollassetsbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28b89-155">Java</span><span class="sxs-lookup"><span data-stu-id="28b89-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableasset-unenrollassetsbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28b89-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b89-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

