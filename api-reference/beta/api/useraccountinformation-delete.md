---
title: Excluir userAccountInformation
description: Excluir um objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 090df364dd86f2ab47b02259ff81acc36ad0aa6d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938145"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="34579-103">Excluir userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="34579-103">Delete userAccountInformation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34579-104">Excluir um objeto [userAccountInformation](../resources/useraccountinformation.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="34579-104">Delete a [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34579-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34579-105">Permissions</span></span>

<span data-ttu-id="34579-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34579-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34579-108">Permission type</span></span>                        | <span data-ttu-id="34579-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34579-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34579-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34579-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="34579-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34579-111">Not supported.</span></span>                              |
| <span data-ttu-id="34579-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34579-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34579-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34579-113">Not supported.</span></span>                              |
| <span data-ttu-id="34579-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34579-114">Application</span></span>                            | <span data-ttu-id="34579-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34579-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="34579-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34579-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /user/profile/account{id}
```

## <a name="request-headers"></a><span data-ttu-id="34579-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34579-117">Request headers</span></span>

| <span data-ttu-id="34579-118">Nome</span><span class="sxs-lookup"><span data-stu-id="34579-118">Name</span></span>           |<span data-ttu-id="34579-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="34579-119">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="34579-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="34579-120">Authorization</span></span>  | <span data-ttu-id="34579-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34579-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34579-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34579-123">Request body</span></span>

<span data-ttu-id="34579-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34579-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34579-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="34579-125">Response</span></span>

<span data-ttu-id="34579-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34579-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34579-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="34579-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34579-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34579-129">Request</span></span>

<span data-ttu-id="34579-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34579-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="34579-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="34579-131">Response</span></span>

<span data-ttu-id="34579-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34579-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
