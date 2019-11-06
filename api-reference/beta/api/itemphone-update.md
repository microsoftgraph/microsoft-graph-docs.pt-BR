---
title: Atualizar o número de telefone
description: Atualiza as propriedades de um objeto MyPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b93d76dabf1aef7b45e77fd9a3020fb5da96ab01
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997322"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="0f677-103">Atualizar itemphonenumber</span><span class="sxs-lookup"><span data-stu-id="0f677-103">Update itemphonenumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f677-104">Atualizar as propriedades de um objeto [MyPhone](../resources/itemphone.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0f677-104">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f677-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f677-105">Permissions</span></span>

<span data-ttu-id="0f677-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f677-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f677-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f677-108">Permission type</span></span>                        | <span data-ttu-id="0f677-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f677-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f677-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f677-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f677-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0f677-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0f677-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f677-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f677-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0f677-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0f677-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f677-114">Application</span></span>                            | <span data-ttu-id="0f677-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f677-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0f677-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f677-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/phones/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="0f677-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f677-117">Request headers</span></span>

| <span data-ttu-id="0f677-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0f677-118">Name</span></span>           |<span data-ttu-id="0f677-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f677-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0f677-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f677-120">Authorization</span></span>  | <span data-ttu-id="0f677-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f677-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0f677-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f677-123">Content-Type</span></span>   | <span data-ttu-id="0f677-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f677-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f677-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f677-126">Request body</span></span>

<span data-ttu-id="0f677-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0f677-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0f677-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0f677-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0f677-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0f677-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0f677-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f677-130">Property</span></span>     | <span data-ttu-id="0f677-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f677-131">Type</span></span>        | <span data-ttu-id="0f677-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f677-132">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0f677-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0f677-133">displayName</span></span>   |<span data-ttu-id="0f677-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f677-134">String</span></span>       | <span data-ttu-id="0f677-135">Contém um nome amigável para o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="0f677-135">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="0f677-136">number</span><span class="sxs-lookup"><span data-stu-id="0f677-136">number</span></span>        |<span data-ttu-id="0f677-137">String</span><span class="sxs-lookup"><span data-stu-id="0f677-137">String</span></span>       | <span data-ttu-id="0f677-138">Contém o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="0f677-138">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="0f677-139">type</span><span class="sxs-lookup"><span data-stu-id="0f677-139">type</span></span>          |<span data-ttu-id="0f677-140">string</span><span class="sxs-lookup"><span data-stu-id="0f677-140">string</span></span>       | <span data-ttu-id="0f677-141">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="0f677-141">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="0f677-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f677-142">Response</span></span>

<span data-ttu-id="0f677-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [MyPhone](../resources/itemphone.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f677-143">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f677-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f677-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f677-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f677-145">Request</span></span>

<span data-ttu-id="0f677-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f677-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0f677-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f677-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f677-148">C#</span><span class="sxs-lookup"><span data-stu-id="0f677-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f677-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f677-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f677-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f677-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f677-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f677-151">Response</span></span>

<span data-ttu-id="0f677-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f677-152">The following is an example of the response.</span></span>

> <span data-ttu-id="0f677-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f677-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
