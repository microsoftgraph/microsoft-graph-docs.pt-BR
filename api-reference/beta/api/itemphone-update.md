---
title: Atualizar o número de telefone
description: Atualiza as propriedades de um objeto MyPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4b1dd50e9448c4b6aa06b8e29609327678cae228
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229014"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="6348a-103">Atualizar itemphonenumber</span><span class="sxs-lookup"><span data-stu-id="6348a-103">Update itemphonenumber</span></span>

<span data-ttu-id="6348a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6348a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6348a-105">Atualizar as propriedades de um objeto [MyPhone](../resources/itemphone.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6348a-105">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6348a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6348a-106">Permissions</span></span>

<span data-ttu-id="6348a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6348a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6348a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6348a-109">Permission type</span></span>                        | <span data-ttu-id="6348a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6348a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6348a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6348a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6348a-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6348a-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6348a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6348a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6348a-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6348a-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6348a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6348a-115">Application</span></span>                            | <span data-ttu-id="6348a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6348a-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="6348a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6348a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6348a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6348a-118">Request headers</span></span>

| <span data-ttu-id="6348a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6348a-119">Name</span></span>           |<span data-ttu-id="6348a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6348a-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="6348a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6348a-121">Authorization</span></span>  | <span data-ttu-id="6348a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6348a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6348a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6348a-124">Content-Type</span></span>   | <span data-ttu-id="6348a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6348a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6348a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6348a-127">Request body</span></span>

<span data-ttu-id="6348a-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6348a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6348a-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6348a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6348a-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6348a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6348a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6348a-131">Property</span></span>     | <span data-ttu-id="6348a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6348a-132">Type</span></span>        | <span data-ttu-id="6348a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6348a-133">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6348a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6348a-134">displayName</span></span>   |<span data-ttu-id="6348a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6348a-135">String</span></span>       | <span data-ttu-id="6348a-136">Contém um nome amigável para o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="6348a-136">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="6348a-137">number</span><span class="sxs-lookup"><span data-stu-id="6348a-137">number</span></span>        |<span data-ttu-id="6348a-138">String</span><span class="sxs-lookup"><span data-stu-id="6348a-138">String</span></span>       | <span data-ttu-id="6348a-139">Contém o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="6348a-139">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="6348a-140">type</span><span class="sxs-lookup"><span data-stu-id="6348a-140">type</span></span>          |<span data-ttu-id="6348a-141">string</span><span class="sxs-lookup"><span data-stu-id="6348a-141">string</span></span>       | <span data-ttu-id="6348a-142">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="6348a-142">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="6348a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6348a-143">Response</span></span>

<span data-ttu-id="6348a-144">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [MyPhone](../resources/itemphone.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6348a-144">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6348a-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6348a-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6348a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6348a-146">Request</span></span>

<span data-ttu-id="6348a-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6348a-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6348a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6348a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/phones/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6348a-149">C#</span><span class="sxs-lookup"><span data-stu-id="6348a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6348a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6348a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6348a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6348a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6348a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6348a-152">Response</span></span>

<span data-ttu-id="6348a-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6348a-153">The following is an example of the response.</span></span>

> <span data-ttu-id="6348a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6348a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itemphone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
