---
title: Excluir foto
description: Exclua uma foto.
localization_priority: Normal
ms.openlocfilehash: e83e00f6579c300395b21608c89984a775bb5ab4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830552"
---
# <a name="delete-photo"></a><span data-ttu-id="baaac-103">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="baaac-103">Delete photo</span></span>

<span data-ttu-id="baaac-104">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="baaac-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="baaac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="baaac-105">Permissions</span></span>
<span data-ttu-id="baaac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baaac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baaac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baaac-108">Permission type</span></span>      | <span data-ttu-id="baaac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="baaac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baaac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baaac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="baaac-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baaac-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="baaac-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baaac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baaac-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baaac-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="baaac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baaac-114">Application</span></span> | <span data-ttu-id="baaac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baaac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="baaac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baaac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="baaac-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baaac-117">Request headers</span></span>
| <span data-ttu-id="baaac-118">Nome</span><span class="sxs-lookup"><span data-stu-id="baaac-118">Name</span></span>       | <span data-ttu-id="baaac-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="baaac-119">Type</span></span> | <span data-ttu-id="baaac-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="baaac-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="baaac-121">if-match</span><span class="sxs-lookup"><span data-stu-id="baaac-121">if-match</span></span>  | <span data-ttu-id="baaac-122">string</span><span class="sxs-lookup"><span data-stu-id="baaac-122">string</span></span>  | <span data-ttu-id="baaac-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="baaac-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="baaac-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="baaac-124">Authorization</span></span>  | <span data-ttu-id="baaac-125">string</span><span class="sxs-lookup"><span data-stu-id="baaac-125">string</span></span>  | <span data-ttu-id="baaac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baaac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="baaac-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baaac-128">Request body</span></span>
<span data-ttu-id="baaac-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="baaac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baaac-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="baaac-130">Response</span></span>

<span data-ttu-id="baaac-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baaac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baaac-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baaac-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="baaac-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baaac-134">Request</span></span>
<span data-ttu-id="baaac-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baaac-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="baaac-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="baaac-136">Response</span></span>
<span data-ttu-id="baaac-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baaac-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
