---
title: Atualizar personAnniversary
description: Atualize as propriedades do objeto personanniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 938d0ef37b26221b5cdec958cff1a1bb53576ab5
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997264"
---
# <a name="update-personanniversary"></a><span data-ttu-id="b4a7b-103">Atualizar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="b4a7b-103">Update personAnniversary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4a7b-104">Atualiza as propriedades de um objeto [personAnniversary](../resources/personanniversary.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-104">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4a7b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4a7b-105">Permissions</span></span>

<span data-ttu-id="b4a7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4a7b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4a7b-108">Permission type</span></span>                        | <span data-ttu-id="b4a7b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4a7b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4a7b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4a7b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4a7b-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b4a7b-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b4a7b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4a7b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4a7b-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b4a7b-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b4a7b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4a7b-114">Application</span></span>                            | <span data-ttu-id="b4a7b-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a7b-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b4a7b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4a7b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="b4a7b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a7b-117">Request headers</span></span>

| <span data-ttu-id="b4a7b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b4a7b-118">Name</span></span>           |<span data-ttu-id="b4a7b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a7b-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b4a7b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4a7b-120">Authorization</span></span>  | <span data-ttu-id="b4a7b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b4a7b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4a7b-123">Content-Type</span></span>   | <span data-ttu-id="b4a7b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4a7b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a7b-126">Request body</span></span>

<span data-ttu-id="b4a7b-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b4a7b-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b4a7b-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4a7b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4a7b-130">Property</span></span>     | <span data-ttu-id="b4a7b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4a7b-131">Type</span></span>        | <span data-ttu-id="b4a7b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a7b-132">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="b4a7b-133">data</span><span class="sxs-lookup"><span data-stu-id="b4a7b-133">date</span></span>          |<span data-ttu-id="b4a7b-134">Data</span><span class="sxs-lookup"><span data-stu-id="b4a7b-134">Date</span></span>         | <span data-ttu-id="b4a7b-135">Contém a data associada ao tipo de aniversário.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-135">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="b4a7b-136">type</span><span class="sxs-lookup"><span data-stu-id="b4a7b-136">type</span></span>          |<span data-ttu-id="b4a7b-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4a7b-137">string</span></span>       | <span data-ttu-id="b4a7b-138">Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-138">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="b4a7b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4a7b-139">Response</span></span>

<span data-ttu-id="b4a7b-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [personAnniversary](../resources/personanniversary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-140">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4a7b-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b4a7b-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4a7b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a7b-142">Request</span></span>

<span data-ttu-id="b4a7b-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-143">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b4a7b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4a7b-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4a7b-145">C#</span><span class="sxs-lookup"><span data-stu-id="b4a7b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4a7b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4a7b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4a7b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4a7b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4a7b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4a7b-148">Response</span></span>

<span data-ttu-id="b4a7b-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-149">The following is an example of the response.</span></span>

> <span data-ttu-id="b4a7b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4a7b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
