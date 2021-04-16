---
title: checkMemberGroups
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d76b252fcf6c4239c598a4f6591ae2392d25cdba
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869950"
---
# <a name="checkmembergroups"></a><span data-ttu-id="772ca-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="772ca-104">checkMemberGroups</span></span>

<span data-ttu-id="772ca-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="772ca-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="772ca-p102">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="772ca-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="772ca-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Microsoft 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Microsoft 365 não podem conter grupos, então associações em um Grupo do Microsoft 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="772ca-p103">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="772ca-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="772ca-112">Permissions</span></span>

<span data-ttu-id="772ca-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="772ca-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="772ca-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="772ca-115">Permission type</span></span>                        | <span data-ttu-id="772ca-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="772ca-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="772ca-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="772ca-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="772ca-118">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="772ca-118">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="772ca-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="772ca-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="772ca-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="772ca-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="772ca-121">Application</span><span class="sxs-lookup"><span data-stu-id="772ca-121">Application</span></span>                            | <span data-ttu-id="772ca-122">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="772ca-122">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="772ca-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="772ca-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="772ca-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="772ca-124">Request headers</span></span>

| <span data-ttu-id="772ca-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="772ca-125">Header</span></span>        | <span data-ttu-id="772ca-126">Valor</span><span class="sxs-lookup"><span data-stu-id="772ca-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="772ca-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="772ca-127">Authorization</span></span> | <span data-ttu-id="772ca-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="772ca-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="772ca-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="772ca-130">Content-Type</span></span>  | <span data-ttu-id="772ca-131">application/json</span><span class="sxs-lookup"><span data-stu-id="772ca-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="772ca-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="772ca-132">Request body</span></span>

<span data-ttu-id="772ca-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="772ca-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="772ca-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="772ca-134">Parameter</span></span> | <span data-ttu-id="772ca-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="772ca-135">Type</span></span>              | <span data-ttu-id="772ca-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="772ca-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="772ca-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="772ca-137">groupIds</span></span>  | <span data-ttu-id="772ca-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="772ca-138">String collection</span></span> | <span data-ttu-id="772ca-139">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="772ca-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="772ca-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="772ca-140">Response</span></span>

<span data-ttu-id="772ca-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="772ca-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="772ca-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="772ca-142">Example</span></span>

<span data-ttu-id="772ca-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="772ca-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="772ca-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="772ca-144">Request</span></span>

<span data-ttu-id="772ca-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="772ca-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="772ca-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="772ca-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="772ca-147">C#</span><span class="sxs-lookup"><span data-stu-id="772ca-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="772ca-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="772ca-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="772ca-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="772ca-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="772ca-150">Java</span><span class="sxs-lookup"><span data-stu-id="772ca-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="772ca-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="772ca-151">Response</span></span>

<span data-ttu-id="772ca-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="772ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

