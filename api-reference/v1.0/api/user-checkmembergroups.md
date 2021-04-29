---
title: checkMemberGroups
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 28c4833bc6b3e83f957d113fc5c088abb1696083
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52033640"
---
# <a name="checkmembergroups"></a><span data-ttu-id="5962c-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="5962c-104">checkMemberGroups</span></span>

<span data-ttu-id="5962c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5962c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5962c-p102">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="5962c-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="5962c-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Microsoft 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Microsoft 365 não podem conter grupos, então associações em um Grupo do Microsoft 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="5962c-p103">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="5962c-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="5962c-112">Permissions</span></span>

<span data-ttu-id="5962c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5962c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5962c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5962c-115">Permission type</span></span>                        | <span data-ttu-id="5962c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5962c-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5962c-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5962c-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="5962c-118">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5962c-118">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="5962c-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5962c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5962c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5962c-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="5962c-121">Application</span><span class="sxs-lookup"><span data-stu-id="5962c-121">Application</span></span>                            | <span data-ttu-id="5962c-122">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5962c-122">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5962c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5962c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="5962c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5962c-124">Request headers</span></span>

| <span data-ttu-id="5962c-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5962c-125">Header</span></span>        | <span data-ttu-id="5962c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="5962c-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="5962c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="5962c-127">Authorization</span></span> | <span data-ttu-id="5962c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5962c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5962c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5962c-130">Content-Type</span></span>  | <span data-ttu-id="5962c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5962c-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="5962c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5962c-132">Request body</span></span>

<span data-ttu-id="5962c-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5962c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5962c-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5962c-134">Parameter</span></span> | <span data-ttu-id="5962c-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="5962c-135">Type</span></span>              | <span data-ttu-id="5962c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5962c-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="5962c-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="5962c-137">groupIds</span></span>  | <span data-ttu-id="5962c-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5962c-138">String collection</span></span> | <span data-ttu-id="5962c-139">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="5962c-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="5962c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5962c-140">Response</span></span>

<span data-ttu-id="5962c-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5962c-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5962c-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5962c-142">Example</span></span>

<span data-ttu-id="5962c-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5962c-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5962c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5962c-144">Request</span></span>

<span data-ttu-id="5962c-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5962c-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5962c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5962c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="5962c-147">C#</span><span class="sxs-lookup"><span data-stu-id="5962c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5962c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5962c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5962c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5962c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5962c-150">Java</span><span class="sxs-lookup"><span data-stu-id="5962c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5962c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5962c-151">Response</span></span>

<span data-ttu-id="5962c-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5962c-152">Here is an example of the response.</span></span> <span data-ttu-id="5962c-153">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5962c-153">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

