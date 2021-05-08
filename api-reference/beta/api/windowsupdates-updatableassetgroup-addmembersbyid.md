---
title: 'updatableAssetGroup: addMembersById'
description: Adicione membros do mesmo tipo a um updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 27585b3ad87c4154140024705227612a988c7a76
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239477"
---
# <a name="updatableassetgroup-addmembersbyid"></a><span data-ttu-id="486cf-103">updatableAssetGroup: addMembersById</span><span class="sxs-lookup"><span data-stu-id="486cf-103">updatableAssetGroup: addMembersById</span></span>
<span data-ttu-id="486cf-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="486cf-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="486cf-105">Adicione membros do mesmo tipo a um [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="486cf-105">Add members of the same type to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="486cf-106">Você também pode usar os [addMembers do método](windowsupdates-updatableassetgroup-addmembers.md) para adicionar membros.</span><span class="sxs-lookup"><span data-stu-id="486cf-106">You can also use the method [addMembers](windowsupdates-updatableassetgroup-addmembers.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="486cf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="486cf-107">Permissions</span></span>
<span data-ttu-id="486cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="486cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="486cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="486cf-110">Permission type</span></span>|<span data-ttu-id="486cf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="486cf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="486cf-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="486cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="486cf-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="486cf-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="486cf-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="486cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="486cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="486cf-115">Not supported.</span></span>|
|<span data-ttu-id="486cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="486cf-116">Application</span></span>|<span data-ttu-id="486cf-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="486cf-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="486cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="486cf-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
```

## <a name="request-headers"></a><span data-ttu-id="486cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="486cf-119">Request headers</span></span>
|<span data-ttu-id="486cf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="486cf-120">Name</span></span>|<span data-ttu-id="486cf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="486cf-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="486cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="486cf-122">Authorization</span></span>|<span data-ttu-id="486cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="486cf-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="486cf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="486cf-125">Content-Type</span></span>|<span data-ttu-id="486cf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="486cf-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="486cf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="486cf-128">Request body</span></span>
<span data-ttu-id="486cf-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="486cf-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="486cf-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="486cf-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="486cf-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="486cf-131">Parameter</span></span>|<span data-ttu-id="486cf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="486cf-132">Type</span></span>|<span data-ttu-id="486cf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="486cf-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="486cf-134">ids</span><span class="sxs-lookup"><span data-stu-id="486cf-134">ids</span></span>|<span data-ttu-id="486cf-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="486cf-135">String collection</span></span>|<span data-ttu-id="486cf-136">Lista de identificadores correspondentes aos [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) a adicionar como membros do **updatableAssetGroup**.</span><span class="sxs-lookup"><span data-stu-id="486cf-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="486cf-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="486cf-137">memberEntityType</span></span>|<span data-ttu-id="486cf-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="486cf-138">String</span></span>|<span data-ttu-id="486cf-139">O tipo completo dos **recursos updatableAsset.**</span><span class="sxs-lookup"><span data-stu-id="486cf-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="486cf-140">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="486cf-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="486cf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="486cf-141">Response</span></span>

<span data-ttu-id="486cf-142">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="486cf-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="486cf-143">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="486cf-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="486cf-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="486cf-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="486cf-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="486cf-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="486cf-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="486cf-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
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
# <a name="c"></a>[<span data-ttu-id="486cf-147">C#</span><span class="sxs-lookup"><span data-stu-id="486cf-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableassetgroup-addmembersbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="486cf-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="486cf-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableassetgroup-addmembersbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="486cf-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="486cf-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableassetgroup-addmembersbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="486cf-150">Java</span><span class="sxs-lookup"><span data-stu-id="486cf-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableassetgroup-addmembersbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="486cf-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="486cf-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

