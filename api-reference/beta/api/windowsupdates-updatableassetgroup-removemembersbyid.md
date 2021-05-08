---
title: 'updatableAssetGroup: removeMembersById'
description: Remova membros do mesmo tipo de um updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: dde1a86c363a2c8b7fe3492316bdcf5fc3593f26
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239033"
---
# <a name="updatableassetgroup-removemembersbyid"></a><span data-ttu-id="12197-103">updatableAssetGroup: removeMembersById</span><span class="sxs-lookup"><span data-stu-id="12197-103">updatableAssetGroup: removeMembersById</span></span>
<span data-ttu-id="12197-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="12197-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12197-105">Remover membros do mesmo tipo de um [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="12197-105">Remove members of the same type from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="12197-106">Você também pode usar o [método removeMembers para](windowsupdates-updatableassetgroup-removemembers.md) remover membros.</span><span class="sxs-lookup"><span data-stu-id="12197-106">You can also use the method [removeMembers](windowsupdates-updatableassetgroup-removemembers.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="12197-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="12197-107">Permissions</span></span>
<span data-ttu-id="12197-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12197-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12197-110">Permission type</span></span>|<span data-ttu-id="12197-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12197-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12197-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12197-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12197-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12197-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="12197-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12197-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12197-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12197-115">Not supported.</span></span>|
|<span data-ttu-id="12197-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12197-116">Application</span></span>|<span data-ttu-id="12197-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12197-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12197-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12197-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
```

## <a name="request-headers"></a><span data-ttu-id="12197-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12197-119">Request headers</span></span>
|<span data-ttu-id="12197-120">Nome</span><span class="sxs-lookup"><span data-stu-id="12197-120">Name</span></span>|<span data-ttu-id="12197-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="12197-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="12197-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12197-122">Authorization</span></span>|<span data-ttu-id="12197-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12197-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="12197-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12197-125">Content-Type</span></span>|<span data-ttu-id="12197-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12197-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12197-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12197-128">Request body</span></span>
<span data-ttu-id="12197-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="12197-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="12197-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="12197-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="12197-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="12197-131">Parameter</span></span>|<span data-ttu-id="12197-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="12197-132">Type</span></span>|<span data-ttu-id="12197-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="12197-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12197-134">ids</span><span class="sxs-lookup"><span data-stu-id="12197-134">ids</span></span>|<span data-ttu-id="12197-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="12197-135">String collection</span></span>|<span data-ttu-id="12197-136">Lista de identificadores correspondentes aos [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) a remover como membros do **updatableAssetGroup**.</span><span class="sxs-lookup"><span data-stu-id="12197-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to remove as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="12197-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="12197-137">memberEntityType</span></span>|<span data-ttu-id="12197-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12197-138">String</span></span>|<span data-ttu-id="12197-139">O tipo completo dos **recursos updatableAsset.**</span><span class="sxs-lookup"><span data-stu-id="12197-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="12197-140">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="12197-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="12197-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="12197-141">Response</span></span>

<span data-ttu-id="12197-142">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="12197-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="12197-143">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12197-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12197-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="12197-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12197-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12197-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="12197-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="12197-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
Content-Type: application/json

{
  "ids": [
    "String",
    "String",
    "String"
  ],
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice"
}
```
# <a name="c"></a>[<span data-ttu-id="12197-147">C#</span><span class="sxs-lookup"><span data-stu-id="12197-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableassetgroup-removemembersbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12197-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12197-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableassetgroup-removemembersbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12197-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12197-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableassetgroup-removemembersbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12197-150">Java</span><span class="sxs-lookup"><span data-stu-id="12197-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableassetgroup-removemembersbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="12197-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="12197-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

