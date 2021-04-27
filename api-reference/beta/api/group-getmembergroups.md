---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação memberOf, que retorna somente os grupos dos quais o grupo é membro direto.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 97b44b675d48dc07cf4fa11c8413e34a603739f4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041824"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="d0450-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d0450-104">group: getMemberGroups</span></span>

<span data-ttu-id="d0450-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0450-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0450-p102">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group-list-memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="d0450-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="d0450-p103">Esta função é compatível com o Microsoft 365 e outros tipos de grupos provisionados no Azure AD. O número máximo de grupos que cada solicitação pode retornar é 2046. Observe que os grupos do Microsoft 365 não podem conter grupos. Portanto, associações em um grupo do Microsoft 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="d0450-p103">This function supports Microsoft 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0450-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0450-112">Permissions</span></span>

<span data-ttu-id="d0450-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0450-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0450-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0450-115">Permission type</span></span>                        | <span data-ttu-id="d0450-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0450-116">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d0450-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0450-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0450-118">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="d0450-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d0450-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0450-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0450-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0450-120">Not supported.</span></span>                                                                              |
| <span data-ttu-id="d0450-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0450-121">Application</span></span>                            | <span data-ttu-id="d0450-122">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d0450-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="d0450-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0450-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="d0450-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0450-124">Request headers</span></span>

| <span data-ttu-id="d0450-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d0450-125">Name</span></span>          | <span data-ttu-id="d0450-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0450-126">Type</span></span>   | <span data-ttu-id="d0450-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0450-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d0450-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0450-128">Authorization</span></span> | <span data-ttu-id="d0450-129">string</span><span class="sxs-lookup"><span data-stu-id="d0450-129">string</span></span> | <span data-ttu-id="d0450-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0450-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0450-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0450-132">Request body</span></span>

<span data-ttu-id="d0450-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0450-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d0450-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d0450-134">Parameter</span></span>           | <span data-ttu-id="d0450-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0450-135">Type</span></span>    | <span data-ttu-id="d0450-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0450-136">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="d0450-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d0450-137">securityEnabledOnly</span></span> | <span data-ttu-id="d0450-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0450-138">Boolean</span></span> | <span data-ttu-id="d0450-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="d0450-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="d0450-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0450-141">Response</span></span>

<span data-ttu-id="d0450-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="d0450-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="d0450-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0450-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d0450-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0450-144">Request</span></span>

<span data-ttu-id="d0450-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0450-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0450-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0450-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="d0450-147">C#</span><span class="sxs-lookup"><span data-stu-id="d0450-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0450-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0450-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0450-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0450-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0450-150">Java</span><span class="sxs-lookup"><span data-stu-id="d0450-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d0450-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0450-151">Response</span></span>

<span data-ttu-id="d0450-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0450-152">The following is an example of the response.</span></span>

> <span data-ttu-id="d0450-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d0450-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


