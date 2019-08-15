---
author: JeremyKelley
ms.author: jeremyke
title: Excluir pacote
description: Excluir um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7556edc226f655af748facea1df6ea19820b7c9e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419249"
---
# <a name="delete-bundle"></a><span data-ttu-id="46f17-103">Excluir pacote</span><span class="sxs-lookup"><span data-stu-id="46f17-103">Delete bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46f17-104">Excluir um [pacote][] de driveItems usando sua **ID**. Observe que excluir um pacote usando esse método exclui permanentemente o pacote e não o move para a lixeira.</span><span class="sxs-lookup"><span data-stu-id="46f17-104">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="46f17-105">No entanto, ele não remove os itens que foram referenciados pelo pacote.</span><span class="sxs-lookup"><span data-stu-id="46f17-105">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="46f17-106">Eles permanecerão em suas pastas pai.</span><span class="sxs-lookup"><span data-stu-id="46f17-106">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="46f17-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="46f17-107">Permissions</span></span>

<span data-ttu-id="46f17-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46f17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46f17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46f17-110">Permission type</span></span>      | <span data-ttu-id="46f17-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46f17-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46f17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46f17-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46f17-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46f17-113">Not supported.</span></span>                             |
|<span data-ttu-id="46f17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46f17-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46f17-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46f17-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="46f17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46f17-116">Application</span></span>          | <span data-ttu-id="46f17-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46f17-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="46f17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46f17-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="46f17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46f17-119">Request headers</span></span>

| <span data-ttu-id="46f17-120">Nome</span><span class="sxs-lookup"><span data-stu-id="46f17-120">Name</span></span>          | <span data-ttu-id="46f17-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="46f17-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="46f17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46f17-122">Authorization</span></span> | <span data-ttu-id="46f17-123">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="46f17-123">Bearer \{token\}.</span></span> <span data-ttu-id="46f17-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46f17-124">Required.</span></span> |
| <span data-ttu-id="46f17-125">if-match</span><span class="sxs-lookup"><span data-stu-id="46f17-125">if-match</span></span>      | <span data-ttu-id="46f17-126">ETag.</span><span class="sxs-lookup"><span data-stu-id="46f17-126">eTag.</span></span> <span data-ttu-id="46f17-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="46f17-127">Optional.</span></span> <span data-ttu-id="46f17-128">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no pacote, uma `412 Precondition Failed` resposta será retornada e o pacote não será excluído.</span><span class="sxs-lookup"><span data-stu-id="46f17-128">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="46f17-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46f17-129">Request body</span></span>

<span data-ttu-id="46f17-130">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="46f17-130">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="46f17-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="46f17-131">Response</span></span>

<span data-ttu-id="46f17-132">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="46f17-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="46f17-133">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="46f17-133">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="46f17-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46f17-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="46f17-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46f17-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46f17-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="46f17-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46f17-137">C#</span><span class="sxs-lookup"><span data-stu-id="46f17-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46f17-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46f17-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46f17-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="46f17-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46f17-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="46f17-140">Response</span></span>

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
