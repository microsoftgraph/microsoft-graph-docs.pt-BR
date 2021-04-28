---
title: 'driveItem: restaurar'
description: Restaure um driveItem que foi excluído e está atualmente na lixeira.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 391788bccc09876a1bed78da932dd574f1e23cfb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054046"
---
# <a name="driveitem-restore"></a><span data-ttu-id="90b37-103">driveItem: restaurar</span><span class="sxs-lookup"><span data-stu-id="90b37-103">driveItem: restore</span></span>

<span data-ttu-id="90b37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90b37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90b37-105">Restaure [um driveItem](../resources/driveitem.md) que foi excluído e está atualmente na lixeira.</span><span class="sxs-lookup"><span data-stu-id="90b37-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="90b37-106">**OBSERVAÇÃO**: Essa funcionalidade está disponível apenas para OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="90b37-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="90b37-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="90b37-107">Permissions</span></span>

<span data-ttu-id="90b37-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90b37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90b37-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90b37-110">Permission type</span></span>                        | <span data-ttu-id="90b37-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90b37-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90b37-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90b37-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="90b37-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90b37-113">Not supported.</span></span> |
| <span data-ttu-id="90b37-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90b37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90b37-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b37-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="90b37-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90b37-116">Application</span></span>                            | <span data-ttu-id="90b37-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b37-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90b37-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90b37-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="90b37-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90b37-119">Request headers</span></span>

| <span data-ttu-id="90b37-120">Nome</span><span class="sxs-lookup"><span data-stu-id="90b37-120">Name</span></span>          | <span data-ttu-id="90b37-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="90b37-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="90b37-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90b37-122">Authorization</span></span> | <span data-ttu-id="90b37-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90b37-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90b37-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90b37-125">Request body</span></span>

<span data-ttu-id="90b37-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90b37-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90b37-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="90b37-127">Parameter</span></span>     | <span data-ttu-id="90b37-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="90b37-128">Type</span></span>                                         | <span data-ttu-id="90b37-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="90b37-129">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="90b37-130">parentReference</span><span class="sxs-lookup"><span data-stu-id="90b37-130">parentReference</span></span>|[<span data-ttu-id="90b37-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="90b37-131">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="90b37-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90b37-132">Optional.</span></span> <span data-ttu-id="90b37-133">Referência ao item pai ao que o item excluído será restaurado.</span><span class="sxs-lookup"><span data-stu-id="90b37-133">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="90b37-134">nome</span><span class="sxs-lookup"><span data-stu-id="90b37-134">name</span></span>           |<span data-ttu-id="90b37-135">String</span><span class="sxs-lookup"><span data-stu-id="90b37-135">String</span></span>                                        | <span data-ttu-id="90b37-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90b37-136">Optional.</span></span> <span data-ttu-id="90b37-137">O novo nome do item restaurado.</span><span class="sxs-lookup"><span data-stu-id="90b37-137">The new name for the restored item.</span></span> <span data-ttu-id="90b37-138">Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="90b37-138">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="90b37-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b37-139">Response</span></span>

<span data-ttu-id="90b37-140">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [driveItem](../resources/driveitem.md) restaurado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90b37-140">If successful, this method returns a `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90b37-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90b37-141">Examples</span></span>

<span data-ttu-id="90b37-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="90b37-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="90b37-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90b37-143">Request</span></span>

<span data-ttu-id="90b37-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90b37-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90b37-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="90b37-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "restore-item",
  "scopes": "files.readwrite",
  "target": "action"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{item-id}/restore
Content-type: application/json

{
  "parentReference": {
    "id": "String",
  },
  "name": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="90b37-146">C#</span><span class="sxs-lookup"><span data-stu-id="90b37-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90b37-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90b37-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90b37-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90b37-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90b37-149">Java</span><span class="sxs-lookup"><span data-stu-id="90b37-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90b37-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b37-150">Response</span></span>

<span data-ttu-id="90b37-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90b37-151">The following is an example of the response.</span></span>

> <span data-ttu-id="90b37-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="90b37-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "new-restored-item-name.txt",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Restore a DriveItem.",
  "keywords": "retore,item,driveitem",
  "section": "documentation",
  "tocPath": "Items/Restore"
}-->

