---
title: Atualizar personInterest
description: Atualize as propriedades do objeto personinterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 36b4a9ee685678597e1ba809c163e93a3f77416f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998096"
---
# <a name="update-personinterest"></a><span data-ttu-id="0fb3f-103">Atualizar personinterest</span><span class="sxs-lookup"><span data-stu-id="0fb3f-103">Update personinterest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fb3f-104">Atualiza as propriedades de um objeto [personInterest](../resources/personinterest.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-104">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fb3f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fb3f-105">Permissions</span></span>

<span data-ttu-id="0fb3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fb3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fb3f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fb3f-108">Permission type</span></span>                        | <span data-ttu-id="0fb3f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fb3f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0fb3f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fb3f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fb3f-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0fb3f-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0fb3f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fb3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fb3f-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0fb3f-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0fb3f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fb3f-114">Application</span></span>                            | <span data-ttu-id="0fb3f-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb3f-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0fb3f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb3f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0fb3f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb3f-117">Request headers</span></span>

| <span data-ttu-id="0fb3f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0fb3f-118">Name</span></span>           |<span data-ttu-id="0fb3f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fb3f-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0fb3f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fb3f-120">Authorization</span></span>  | <span data-ttu-id="0fb3f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0fb3f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fb3f-123">Content-Type</span></span>   | <span data-ttu-id="0fb3f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fb3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb3f-126">Request body</span></span>

<span data-ttu-id="0fb3f-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0fb3f-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0fb3f-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0fb3f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fb3f-130">Property</span></span>     | <span data-ttu-id="0fb3f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fb3f-131">Type</span></span>             | <span data-ttu-id="0fb3f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fb3f-132">Description</span></span>                                                                         |
|:-------------|:-----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="0fb3f-133">categories</span><span class="sxs-lookup"><span data-stu-id="0fb3f-133">categories</span></span>    |<span data-ttu-id="0fb3f-134">String collection</span><span class="sxs-lookup"><span data-stu-id="0fb3f-134">String collection</span></span> | <span data-ttu-id="0fb3f-135">Contém categorias que um usuário associou aos juros (por exemplo: pessoal, recipies)</span><span class="sxs-lookup"><span data-stu-id="0fb3f-135">Contains categories a user has associated with the interest (eg: personal, recipies)</span></span>|
|<span data-ttu-id="0fb3f-136">description</span><span class="sxs-lookup"><span data-stu-id="0fb3f-136">description</span></span>   |<span data-ttu-id="0fb3f-137">String</span><span class="sxs-lookup"><span data-stu-id="0fb3f-137">String</span></span>            | <span data-ttu-id="0fb3f-138">Contém uma descrição dos juros.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-138">Contains a description of the interest.</span></span>                                             |
|<span data-ttu-id="0fb3f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0fb3f-139">displayName</span></span>   |<span data-ttu-id="0fb3f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fb3f-140">String</span></span>            | <span data-ttu-id="0fb3f-141">Contém um nome amigável para os juros.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-141">Contains a friendly name for the interest.</span></span>                                          |
|<span data-ttu-id="0fb3f-142">webUrl</span><span class="sxs-lookup"><span data-stu-id="0fb3f-142">webUrl</span></span>        |<span data-ttu-id="0fb3f-143">String</span><span class="sxs-lookup"><span data-stu-id="0fb3f-143">String</span></span>            | <span data-ttu-id="0fb3f-144">Contém um link para uma fonte de informações sobre os juros.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-144">Contains a link to an information source about the interest.</span></span>                        |

## <a name="response"></a><span data-ttu-id="0fb3f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb3f-145">Response</span></span>

<span data-ttu-id="0fb3f-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [personInterest](../resources/personinterest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-146">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fb3f-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0fb3f-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0fb3f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb3f-148">Request</span></span>

<span data-ttu-id="0fb3f-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-149">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fb3f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb3f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personinterest"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/interests/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fb3f-151">C#</span><span class="sxs-lookup"><span data-stu-id="0fb3f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fb3f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fb3f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fb3f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fb3f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0fb3f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb3f-154">Response</span></span>

<span data-ttu-id="0fb3f-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-155">The following is an example of the response.</span></span>

> <span data-ttu-id="0fb3f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personinterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
