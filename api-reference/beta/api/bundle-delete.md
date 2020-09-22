---
author: JeremyKelley
ms.author: jeremyke
title: Excluir pacote
description: Excluir um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 13cc2dcb3cda7dac8d6f9b7acfae153d84efabfa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987768"
---
# <a name="delete-bundle"></a><span data-ttu-id="f35a4-103">Excluir pacote</span><span class="sxs-lookup"><span data-stu-id="f35a4-103">Delete bundle</span></span>

<span data-ttu-id="f35a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f35a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f35a4-105">Excluir um [pacote][] de driveItems usando sua **ID**. Observe que excluir um pacote usando esse método exclui permanentemente o pacote e não o move para a lixeira.</span><span class="sxs-lookup"><span data-stu-id="f35a4-105">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="f35a4-106">No entanto, ele não remove os itens que foram referenciados pelo pacote.</span><span class="sxs-lookup"><span data-stu-id="f35a4-106">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="f35a4-107">Eles permanecerão em suas pastas pai.</span><span class="sxs-lookup"><span data-stu-id="f35a4-107">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="f35a4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f35a4-108">Permissions</span></span>

<span data-ttu-id="f35a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f35a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f35a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f35a4-111">Permission type</span></span>      | <span data-ttu-id="f35a4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f35a4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f35a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f35a4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f35a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f35a4-114">Not supported.</span></span>                             |
|<span data-ttu-id="f35a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f35a4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f35a4-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f35a4-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="f35a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f35a4-117">Application</span></span>          | <span data-ttu-id="f35a4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f35a4-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="f35a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f35a4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="f35a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f35a4-120">Request headers</span></span>

| <span data-ttu-id="f35a4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f35a4-121">Name</span></span>          | <span data-ttu-id="f35a4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f35a4-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="f35a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f35a4-123">Authorization</span></span> | <span data-ttu-id="f35a4-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="f35a4-124">Bearer \{token\}.</span></span> <span data-ttu-id="f35a4-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f35a4-125">Required.</span></span> |
| <span data-ttu-id="f35a4-126">if-match</span><span class="sxs-lookup"><span data-stu-id="f35a4-126">if-match</span></span>      | <span data-ttu-id="f35a4-127">ETag.</span><span class="sxs-lookup"><span data-stu-id="f35a4-127">eTag.</span></span> <span data-ttu-id="f35a4-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f35a4-128">Optional.</span></span> <span data-ttu-id="f35a4-129">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no pacote, uma `412 Precondition Failed` resposta será retornada e o pacote não será excluído.</span><span class="sxs-lookup"><span data-stu-id="f35a4-129">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="f35a4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f35a4-130">Request body</span></span>

<span data-ttu-id="f35a4-131">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="f35a4-131">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="f35a4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f35a4-132">Response</span></span>

<span data-ttu-id="f35a4-133">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="f35a4-133">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="f35a4-134">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="f35a4-134">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="f35a4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f35a4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="f35a4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f35a4-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f35a4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f35a4-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="f35a4-138">C#</span><span class="sxs-lookup"><span data-stu-id="f35a4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f35a4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f35a4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f35a4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f35a4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f35a4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f35a4-141">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath": "Bundles/Delete"
} -->


