---
title: checkMemberGroups
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d26b28a0b94d4316271a217a0e9d73b2d4e78125
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107966"
---
# <a name="checkmembergroups"></a><span data-ttu-id="36282-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="36282-104">checkMemberGroups</span></span>

<span data-ttu-id="36282-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36282-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36282-p102">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="36282-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="36282-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="36282-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="36282-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="36282-112">Permissions</span></span>

<span data-ttu-id="36282-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36282-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36282-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36282-115">Permission type</span></span>                        | <span data-ttu-id="36282-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36282-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="36282-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36282-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="36282-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36282-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="36282-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36282-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36282-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36282-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="36282-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36282-121">Application</span></span>                            | <span data-ttu-id="36282-122">User. Read. All e GroupMember. Read. All, User. Read. All e Group. Read. All, User. ReadWrite. All e GroupMember. Read. All, User. ReadWrite. All e Group. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36282-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36282-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36282-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="36282-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36282-124">Request headers</span></span>

| <span data-ttu-id="36282-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36282-125">Header</span></span>        | <span data-ttu-id="36282-126">Valor</span><span class="sxs-lookup"><span data-stu-id="36282-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="36282-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="36282-127">Authorization</span></span> | <span data-ttu-id="36282-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36282-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36282-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36282-130">Content-Type</span></span>  | <span data-ttu-id="36282-131">application/json</span><span class="sxs-lookup"><span data-stu-id="36282-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="36282-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36282-132">Request body</span></span>

<span data-ttu-id="36282-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36282-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="36282-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="36282-134">Parameter</span></span> | <span data-ttu-id="36282-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="36282-135">Type</span></span>   | <span data-ttu-id="36282-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="36282-136">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="36282-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="36282-137">groupIds</span></span>  | <span data-ttu-id="36282-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="36282-138">String collection</span></span> | <span data-ttu-id="36282-139">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="36282-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="36282-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="36282-140">Response</span></span>

<span data-ttu-id="36282-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36282-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36282-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36282-142">Example</span></span>

<span data-ttu-id="36282-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="36282-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="36282-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36282-144">Request</span></span>

<span data-ttu-id="36282-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36282-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36282-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="36282-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="36282-147">C#</span><span class="sxs-lookup"><span data-stu-id="36282-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36282-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36282-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36282-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36282-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36282-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="36282-150">Response</span></span>

<span data-ttu-id="36282-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36282-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
