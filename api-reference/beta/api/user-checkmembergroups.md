---
title: checkMemberGroups
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4fee17b7f01299c6f35eb056fb1a8bc8b4ce4a85
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409167"
---
# <a name="checkmembergroups"></a><span data-ttu-id="6a725-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="6a725-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a725-p102">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="6a725-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="6a725-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="6a725-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a725-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a725-111">Permissions</span></span>

<span data-ttu-id="6a725-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a725-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a725-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a725-114">Permission type</span></span>                        | <span data-ttu-id="6a725-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a725-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6a725-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a725-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a725-117">User. ReadBasic. All e Group. Read. All, User. Read. All e Group. Read. All, User. ReadWrite. All e Group. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6a725-117">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6a725-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a725-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a725-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a725-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="6a725-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a725-120">Application</span></span>                            | <span data-ttu-id="6a725-121">User. Read. All e Group. Read. All, User. ReadWrite. All e Group. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a725-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a725-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a725-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="6a725-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a725-123">Request headers</span></span>

| <span data-ttu-id="6a725-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a725-124">Header</span></span>        | <span data-ttu-id="6a725-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6a725-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6a725-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a725-126">Authorization</span></span> | <span data-ttu-id="6a725-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a725-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a725-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a725-129">Content-Type</span></span>  | <span data-ttu-id="6a725-130">application/json</span><span class="sxs-lookup"><span data-stu-id="6a725-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="6a725-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a725-131">Request body</span></span>

<span data-ttu-id="6a725-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a725-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6a725-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6a725-133">Parameter</span></span> | <span data-ttu-id="6a725-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a725-134">Type</span></span>   | <span data-ttu-id="6a725-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a725-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="6a725-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="6a725-136">groupIds</span></span>  | <span data-ttu-id="6a725-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a725-137">String collection</span></span> | <span data-ttu-id="6a725-138">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="6a725-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="6a725-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a725-139">Response</span></span>

<span data-ttu-id="6a725-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a725-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a725-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a725-141">Example</span></span>

<span data-ttu-id="6a725-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6a725-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6a725-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a725-143">Request</span></span>

<span data-ttu-id="6a725-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a725-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6a725-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a725-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a725-146">C#</span><span class="sxs-lookup"><span data-stu-id="6a725-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a725-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a725-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a725-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6a725-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6a725-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a725-149">Response</span></span>

<span data-ttu-id="6a725-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a725-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
