---
title: checkMemberGroups
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 41da2d19044bb55fd5ebf8e18c31b267afc3b895
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867892"
---
# <a name="checkmembergroups"></a><span data-ttu-id="b9bff-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b9bff-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9bff-p102">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="b9bff-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="b9bff-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="b9bff-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9bff-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9bff-111">Permissions</span></span>

<span data-ttu-id="b9bff-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9bff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9bff-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9bff-114">Permission type</span></span>                        | <span data-ttu-id="b9bff-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9bff-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b9bff-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9bff-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9bff-117">User. ReadBasic. All e Group. Read. All, User. Read. All e Group. Read. All, User. ReadWrite. All e Group. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b9bff-117">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b9bff-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9bff-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9bff-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9bff-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="b9bff-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9bff-120">Application</span></span>                            | <span data-ttu-id="b9bff-121">User. Read. All e Group. Read. All, User. ReadWrite. All e Group. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b9bff-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9bff-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9bff-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="b9bff-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9bff-123">Request headers</span></span>

| <span data-ttu-id="b9bff-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9bff-124">Header</span></span>        | <span data-ttu-id="b9bff-125">Valor</span><span class="sxs-lookup"><span data-stu-id="b9bff-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="b9bff-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9bff-126">Authorization</span></span> | <span data-ttu-id="b9bff-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9bff-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9bff-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9bff-129">Content-Type</span></span>  | <span data-ttu-id="b9bff-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b9bff-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="b9bff-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9bff-131">Request body</span></span>

<span data-ttu-id="b9bff-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9bff-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9bff-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9bff-133">Parameter</span></span> | <span data-ttu-id="b9bff-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9bff-134">Type</span></span>   | <span data-ttu-id="b9bff-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9bff-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="b9bff-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="b9bff-136">groupIds</span></span>  | <span data-ttu-id="b9bff-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9bff-137">String collection</span></span> | <span data-ttu-id="b9bff-138">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="b9bff-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="b9bff-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9bff-139">Response</span></span>

<span data-ttu-id="b9bff-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9bff-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9bff-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9bff-141">Example</span></span>

<span data-ttu-id="b9bff-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b9bff-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b9bff-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9bff-143">Request</span></span>

<span data-ttu-id="b9bff-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9bff-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b9bff-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9bff-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b9bff-146">C#</span><span class="sxs-lookup"><span data-stu-id="b9bff-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9bff-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="b9bff-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b9bff-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b9bff-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b9bff-149">Java</span><span class="sxs-lookup"><span data-stu-id="b9bff-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9bff-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9bff-150">Response</span></span>

<span data-ttu-id="b9bff-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9bff-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
