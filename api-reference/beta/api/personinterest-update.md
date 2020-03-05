---
title: Atualizar personInterest
description: Atualize as propriedades do objeto personinterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 36d83b710e19c1bcfc92ebae4c61efd2c6fb434b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455904"
---
# <a name="update-personinterest"></a><span data-ttu-id="0dcc0-103">Atualizar personinterest</span><span class="sxs-lookup"><span data-stu-id="0dcc0-103">Update personinterest</span></span>

<span data-ttu-id="0dcc0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0dcc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dcc0-105">Atualiza as propriedades de um objeto [personInterest](../resources/personinterest.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-105">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0dcc0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0dcc0-106">Permissions</span></span>

<span data-ttu-id="0dcc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dcc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0dcc0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dcc0-109">Permission type</span></span>                        | <span data-ttu-id="0dcc0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0dcc0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0dcc0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dcc0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0dcc0-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0dcc0-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0dcc0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dcc0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dcc0-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0dcc0-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0dcc0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dcc0-115">Application</span></span>                            | <span data-ttu-id="0dcc0-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dcc0-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0dcc0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dcc0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0dcc0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dcc0-118">Request headers</span></span>

| <span data-ttu-id="0dcc0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0dcc0-119">Name</span></span>           |<span data-ttu-id="0dcc0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dcc0-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0dcc0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dcc0-121">Authorization</span></span>  | <span data-ttu-id="0dcc0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0dcc0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0dcc0-124">Content-Type</span></span>   | <span data-ttu-id="0dcc0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dcc0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dcc0-127">Request body</span></span>

<span data-ttu-id="0dcc0-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0dcc0-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0dcc0-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0dcc0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dcc0-131">Property</span></span>     | <span data-ttu-id="0dcc0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dcc0-132">Type</span></span>             | <span data-ttu-id="0dcc0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dcc0-133">Description</span></span>                                                                         |
|:-------------|:-----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="0dcc0-134">categories</span><span class="sxs-lookup"><span data-stu-id="0dcc0-134">categories</span></span>    |<span data-ttu-id="0dcc0-135">String collection</span><span class="sxs-lookup"><span data-stu-id="0dcc0-135">String collection</span></span> | <span data-ttu-id="0dcc0-136">Contém categorias que um usuário associou aos juros (por exemplo: pessoal, recipies)</span><span class="sxs-lookup"><span data-stu-id="0dcc0-136">Contains categories a user has associated with the interest (eg: personal, recipies)</span></span>|
|<span data-ttu-id="0dcc0-137">description</span><span class="sxs-lookup"><span data-stu-id="0dcc0-137">description</span></span>   |<span data-ttu-id="0dcc0-138">String</span><span class="sxs-lookup"><span data-stu-id="0dcc0-138">String</span></span>            | <span data-ttu-id="0dcc0-139">Contém uma descrição dos juros.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-139">Contains a description of the interest.</span></span>                                             |
|<span data-ttu-id="0dcc0-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0dcc0-140">displayName</span></span>   |<span data-ttu-id="0dcc0-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dcc0-141">String</span></span>            | <span data-ttu-id="0dcc0-142">Contém um nome amigável para os juros.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-142">Contains a friendly name for the interest.</span></span>                                          |
|<span data-ttu-id="0dcc0-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="0dcc0-143">webUrl</span></span>        |<span data-ttu-id="0dcc0-144">String</span><span class="sxs-lookup"><span data-stu-id="0dcc0-144">String</span></span>            | <span data-ttu-id="0dcc0-145">Contém um link para uma fonte de informações sobre os juros.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-145">Contains a link to an information source about the interest.</span></span>                        |

## <a name="response"></a><span data-ttu-id="0dcc0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dcc0-146">Response</span></span>

<span data-ttu-id="0dcc0-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [personInterest](../resources/personinterest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-147">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0dcc0-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0dcc0-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0dcc0-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dcc0-149">Request</span></span>

<span data-ttu-id="0dcc0-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0dcc0-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dcc0-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0dcc0-152">C#</span><span class="sxs-lookup"><span data-stu-id="0dcc0-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dcc0-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dcc0-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dcc0-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dcc0-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0dcc0-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dcc0-155">Response</span></span>

<span data-ttu-id="0dcc0-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-156">The following is an example of the response.</span></span>

> <span data-ttu-id="0dcc0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0dcc0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
