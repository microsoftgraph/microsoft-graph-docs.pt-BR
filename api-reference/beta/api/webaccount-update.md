---
title: Atualizar webaccount
description: Atualizar as propriedades de um objeto webaccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2a51b252c2fa75695fd62b2d05710a48ce71503c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451522"
---
# <a name="update-webaccount"></a><span data-ttu-id="eebb5-103">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="eebb5-103">Update webAccount</span></span>

<span data-ttu-id="eebb5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eebb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eebb5-105">Atualizar as propriedades de um objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="eebb5-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eebb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eebb5-106">Permissions</span></span>

<span data-ttu-id="eebb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eebb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eebb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eebb5-109">Permission type</span></span>                        | <span data-ttu-id="eebb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eebb5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eebb5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eebb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eebb5-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eebb5-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="eebb5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eebb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eebb5-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eebb5-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="eebb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eebb5-115">Application</span></span>                            | <span data-ttu-id="eebb5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eebb5-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="eebb5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eebb5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eebb5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eebb5-118">Request headers</span></span>

| <span data-ttu-id="eebb5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eebb5-119">Name</span></span>           |<span data-ttu-id="eebb5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eebb5-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="eebb5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eebb5-121">Authorization</span></span>  | <span data-ttu-id="eebb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eebb5-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="eebb5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eebb5-124">Content-Type</span></span>   | <span data-ttu-id="eebb5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eebb5-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="eebb5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eebb5-127">Request body</span></span>

<span data-ttu-id="eebb5-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="eebb5-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="eebb5-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="eebb5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eebb5-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eebb5-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eebb5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eebb5-131">Property</span></span>     | <span data-ttu-id="eebb5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eebb5-132">Type</span></span>                                                    | <span data-ttu-id="eebb5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eebb5-133">Description</span></span>                                                                                     |
|:-------------|:--------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|<span data-ttu-id="eebb5-134">description</span><span class="sxs-lookup"><span data-stu-id="eebb5-134">description</span></span>   |<span data-ttu-id="eebb5-135">String</span><span class="sxs-lookup"><span data-stu-id="eebb5-135">String</span></span>                                                   | <span data-ttu-id="eebb5-136">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="eebb5-136">Contains the description the user has provided for the account on the service being referenced.</span></span> |
|<span data-ttu-id="eebb5-137">service</span><span class="sxs-lookup"><span data-stu-id="eebb5-137">service</span></span>       |[<span data-ttu-id="eebb5-138">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="eebb5-138">serviceInformation</span></span>](../resources/serviceinformation.md) | <span data-ttu-id="eebb5-139">Representa os dados descritivos básicos sobre o serviço de nuvem fornecido por um usuário.</span><span class="sxs-lookup"><span data-stu-id="eebb5-139">Represents the basic descriptive data about cloud service provided by a user.</span></span>                   |
|<span data-ttu-id="eebb5-140">statusMessage</span><span class="sxs-lookup"><span data-stu-id="eebb5-140">statusMessage</span></span> |<span data-ttu-id="eebb5-141">String</span><span class="sxs-lookup"><span data-stu-id="eebb5-141">String</span></span>                                                   | <span data-ttu-id="eebb5-142">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="eebb5-142">Contains a status message from the cloud service if provided or synchronized.</span></span>                   |
|<span data-ttu-id="eebb5-143">userId</span><span class="sxs-lookup"><span data-stu-id="eebb5-143">userId</span></span>        |<span data-ttu-id="eebb5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eebb5-144">String</span></span>                                                   | <span data-ttu-id="eebb5-145">O nome de usuário exibido para a conta da webaccount (por exemplo, @kevinb).</span><span class="sxs-lookup"><span data-stu-id="eebb5-145">The user name  displayed for the webaccount (for example, @kevinb).</span></span>                                       |
|<span data-ttu-id="eebb5-146">webUrl</span><span class="sxs-lookup"><span data-stu-id="eebb5-146">webUrl</span></span>        |<span data-ttu-id="eebb5-147">String</span><span class="sxs-lookup"><span data-stu-id="eebb5-147">String</span></span>                                                   | <span data-ttu-id="eebb5-148">Contém um link para o perfil de usuários no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="eebb5-148">Contains a link to the users profile on the cloud service if one exists.</span></span>                        |

## <a name="response"></a><span data-ttu-id="eebb5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="eebb5-149">Response</span></span>

<span data-ttu-id="eebb5-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [webaccount](../resources/webaccount.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eebb5-150">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eebb5-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eebb5-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eebb5-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eebb5-152">Request</span></span>

<span data-ttu-id="eebb5-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eebb5-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eebb5-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="eebb5-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eebb5-155">C#</span><span class="sxs-lookup"><span data-stu-id="eebb5-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eebb5-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eebb5-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eebb5-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eebb5-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eebb5-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="eebb5-158">Response</span></span>

<span data-ttu-id="eebb5-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eebb5-159">The following is an example of the response.</span></span>

> <span data-ttu-id="eebb5-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eebb5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
