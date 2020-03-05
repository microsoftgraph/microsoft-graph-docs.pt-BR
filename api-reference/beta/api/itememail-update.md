---
title: Atualizar email
description: Atualizar as propriedades de um objeto item de email no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a0d65971de615c788073938819cdfd0d0fb352d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457225"
---
# <a name="update-itememail"></a><span data-ttu-id="d0265-103">Atualizar email</span><span class="sxs-lookup"><span data-stu-id="d0265-103">Update itememail</span></span>

<span data-ttu-id="d0265-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d0265-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0265-105">Atualizar as propriedades de um objeto item de [email](../resources/itememail.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d0265-105">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0265-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0265-106">Permissions</span></span>

<span data-ttu-id="d0265-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0265-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0265-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0265-109">Permission type</span></span>                        | <span data-ttu-id="d0265-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0265-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0265-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0265-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0265-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d0265-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d0265-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0265-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0265-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d0265-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d0265-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0265-115">Application</span></span>                            | <span data-ttu-id="d0265-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0265-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d0265-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0265-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/emails/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="d0265-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0265-118">Request headers</span></span>

| <span data-ttu-id="d0265-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d0265-119">Name</span></span>           |<span data-ttu-id="d0265-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0265-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d0265-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0265-121">Authorization</span></span>  | <span data-ttu-id="d0265-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0265-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d0265-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0265-124">Content-Type</span></span>   | <span data-ttu-id="d0265-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0265-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0265-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0265-127">Request body</span></span>

<span data-ttu-id="d0265-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d0265-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d0265-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d0265-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0265-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d0265-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0265-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0265-131">Property</span></span>     | <span data-ttu-id="d0265-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0265-132">Type</span></span>        | <span data-ttu-id="d0265-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0265-133">Description</span></span>                                                              |
|:-------------|:------------|:-------------------------------------------------------------------------|
|<span data-ttu-id="d0265-134">address</span><span class="sxs-lookup"><span data-stu-id="d0265-134">address</span></span>       |<span data-ttu-id="d0265-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0265-135">String</span></span>       | <span data-ttu-id="d0265-136">O próprio endereço de email.</span><span class="sxs-lookup"><span data-stu-id="d0265-136">The email address itself.</span></span>                                                | 
|<span data-ttu-id="d0265-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d0265-137">displayName</span></span>   |<span data-ttu-id="d0265-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0265-138">String</span></span>       | <span data-ttu-id="d0265-139">O nome ou rótulo que um usuário associou a um endereço de email específico.</span><span class="sxs-lookup"><span data-stu-id="d0265-139">The name or label a user has associated with a particular email address.</span></span> |
|<span data-ttu-id="d0265-140">type</span><span class="sxs-lookup"><span data-stu-id="d0265-140">type</span></span>          |<span data-ttu-id="d0265-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0265-141">string</span></span>       | <span data-ttu-id="d0265-142">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="d0265-142">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>     |

## <a name="response"></a><span data-ttu-id="d0265-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0265-143">Response</span></span>

<span data-ttu-id="d0265-144">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [MyEmail](../resources/itememail.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0265-144">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0265-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0265-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0265-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0265-146">Request</span></span>

<span data-ttu-id="d0265-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0265-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0265-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0265-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/emails/{id}
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d0265-149">C#</span><span class="sxs-lookup"><span data-stu-id="d0265-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0265-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0265-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0265-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0265-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0265-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0265-152">Response</span></span>

<span data-ttu-id="d0265-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0265-153">The following is an example of the response.</span></span>

> <span data-ttu-id="d0265-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0265-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itememail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
