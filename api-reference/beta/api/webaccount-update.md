---
title: Atualizar webaccount
description: Atualizar as propriedades de um objeto webaccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f13a7a350bb3fa2214061c3f8bc1c08a64267223
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996125"
---
# <a name="update-webaccount"></a><span data-ttu-id="74e96-103">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="74e96-103">Update webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74e96-104">Atualizar as propriedades de um objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="74e96-104">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="74e96-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="74e96-105">Permissions</span></span>

<span data-ttu-id="74e96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74e96-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74e96-108">Permission type</span></span>                        | <span data-ttu-id="74e96-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74e96-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="74e96-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74e96-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="74e96-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="74e96-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="74e96-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74e96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e96-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="74e96-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="74e96-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74e96-114">Application</span></span>                            | <span data-ttu-id="74e96-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e96-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="74e96-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74e96-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="74e96-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74e96-117">Request headers</span></span>

| <span data-ttu-id="74e96-118">Nome</span><span class="sxs-lookup"><span data-stu-id="74e96-118">Name</span></span>           |<span data-ttu-id="74e96-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="74e96-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="74e96-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="74e96-120">Authorization</span></span>  | <span data-ttu-id="74e96-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74e96-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="74e96-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74e96-123">Content-Type</span></span>   | <span data-ttu-id="74e96-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74e96-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="74e96-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74e96-126">Request body</span></span>

<span data-ttu-id="74e96-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="74e96-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="74e96-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="74e96-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="74e96-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="74e96-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="74e96-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74e96-130">Property</span></span>     | <span data-ttu-id="74e96-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="74e96-131">Type</span></span>                                                    | <span data-ttu-id="74e96-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="74e96-132">Description</span></span>                                                                                     |
|:-------------|:--------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|<span data-ttu-id="74e96-133">description</span><span class="sxs-lookup"><span data-stu-id="74e96-133">description</span></span>   |<span data-ttu-id="74e96-134">String</span><span class="sxs-lookup"><span data-stu-id="74e96-134">String</span></span>                                                   | <span data-ttu-id="74e96-135">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="74e96-135">Contains the description the user has provided for the account on the service being referenced.</span></span> |
|<span data-ttu-id="74e96-136">service</span><span class="sxs-lookup"><span data-stu-id="74e96-136">service</span></span>       |[<span data-ttu-id="74e96-137">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="74e96-137">serviceInformation</span></span>](../resources/serviceinformation.md) | <span data-ttu-id="74e96-138">Representa os dados descritivos básicos sobre o serviço de nuvem fornecido por um usuário.</span><span class="sxs-lookup"><span data-stu-id="74e96-138">Represents the basic descriptive data about cloud service provided by a user.</span></span>                   |
|<span data-ttu-id="74e96-139">statusMessage</span><span class="sxs-lookup"><span data-stu-id="74e96-139">statusMessage</span></span> |<span data-ttu-id="74e96-140">String</span><span class="sxs-lookup"><span data-stu-id="74e96-140">String</span></span>                                                   | <span data-ttu-id="74e96-141">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="74e96-141">Contains a status message from the cloud service if provided or synchronized.</span></span>                   |
|<span data-ttu-id="74e96-142">userId</span><span class="sxs-lookup"><span data-stu-id="74e96-142">userId</span></span>        |<span data-ttu-id="74e96-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74e96-143">String</span></span>                                                   | <span data-ttu-id="74e96-144">O nome de usuário exibido para a conta da webaccount (por exemplo, @kevinb).</span><span class="sxs-lookup"><span data-stu-id="74e96-144">The user name  displayed for the webaccount (for example, @kevinb).</span></span>                                       |
|<span data-ttu-id="74e96-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="74e96-145">webUrl</span></span>        |<span data-ttu-id="74e96-146">String</span><span class="sxs-lookup"><span data-stu-id="74e96-146">String</span></span>                                                   | <span data-ttu-id="74e96-147">Contém um link para o perfil de usuários no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="74e96-147">Contains a link to the users profile on the cloud service if one exists.</span></span>                        |

## <a name="response"></a><span data-ttu-id="74e96-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e96-148">Response</span></span>

<span data-ttu-id="74e96-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [webaccount](../resources/webaccount.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74e96-149">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74e96-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="74e96-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74e96-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74e96-151">Request</span></span>

<span data-ttu-id="74e96-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74e96-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74e96-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="74e96-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74e96-154">C#</span><span class="sxs-lookup"><span data-stu-id="74e96-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74e96-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74e96-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74e96-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74e96-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74e96-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e96-157">Response</span></span>

<span data-ttu-id="74e96-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74e96-158">The following is an example of the response.</span></span>

> <span data-ttu-id="74e96-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74e96-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update webaccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
