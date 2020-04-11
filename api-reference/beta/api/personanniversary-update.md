---
title: Atualizar personAnniversary
description: Atualize as propriedades do objeto personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 571a298bec352362f0796b953b00a6df010b1ce0
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228742"
---
# <a name="update-personanniversary"></a><span data-ttu-id="6a077-103">Atualizar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="6a077-103">Update personAnniversary</span></span>

<span data-ttu-id="6a077-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a077-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a077-105">Atualiza as propriedades de um objeto [personAnniversary](../resources/personanniversary.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6a077-105">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a077-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a077-106">Permissions</span></span>

<span data-ttu-id="6a077-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a077-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a077-109">Permission type</span></span>                        | <span data-ttu-id="6a077-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a077-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a077-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a077-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a077-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a077-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6a077-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a077-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a077-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a077-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6a077-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a077-115">Application</span></span>                            | <span data-ttu-id="6a077-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a077-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="6a077-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a077-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="6a077-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a077-118">Request headers</span></span>

| <span data-ttu-id="6a077-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6a077-119">Name</span></span>           |<span data-ttu-id="6a077-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a077-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="6a077-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a077-121">Authorization</span></span>  | <span data-ttu-id="6a077-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a077-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6a077-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a077-124">Content-Type</span></span>   | <span data-ttu-id="6a077-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a077-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a077-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a077-127">Request body</span></span>

<span data-ttu-id="6a077-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6a077-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6a077-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6a077-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6a077-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6a077-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6a077-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a077-131">Property</span></span>     | <span data-ttu-id="6a077-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a077-132">Type</span></span>        | <span data-ttu-id="6a077-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a077-133">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="6a077-134">data</span><span class="sxs-lookup"><span data-stu-id="6a077-134">date</span></span>          |<span data-ttu-id="6a077-135">Data</span><span class="sxs-lookup"><span data-stu-id="6a077-135">Date</span></span>         | <span data-ttu-id="6a077-136">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="6a077-136">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="6a077-137">type</span><span class="sxs-lookup"><span data-stu-id="6a077-137">type</span></span>          |<span data-ttu-id="6a077-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a077-138">string</span></span>       | <span data-ttu-id="6a077-139">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6a077-139">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="6a077-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a077-140">Response</span></span>

<span data-ttu-id="6a077-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [personAnniversary](../resources/personanniversary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a077-141">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a077-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a077-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a077-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a077-143">Request</span></span>

<span data-ttu-id="6a077-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a077-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a077-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a077-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6a077-146">C#</span><span class="sxs-lookup"><span data-stu-id="6a077-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a077-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a077-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a077-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a077-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6a077-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a077-149">Response</span></span>

<span data-ttu-id="6a077-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a077-150">The following is an example of the response.</span></span>

> <span data-ttu-id="6a077-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a077-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personanniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
