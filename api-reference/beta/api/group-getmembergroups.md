---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação, que retorna somente os grupos dos quais o grupo é membro direto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d6d799ed2e97e7ee9ad1f3c95a205f19b75f6a5f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657876"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="f8944-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f8944-104">group: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8944-p102">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group-list-memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="f8944-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="f8944-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="f8944-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8944-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8944-111">Permissions</span></span>

<span data-ttu-id="f8944-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8944-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8944-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8944-114">Permission type</span></span>                        | <span data-ttu-id="f8944-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8944-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="f8944-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8944-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8944-117">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f8944-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f8944-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8944-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8944-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8944-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="f8944-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8944-120">Application</span></span>                            | <span data-ttu-id="f8944-121">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8944-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="f8944-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8944-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="f8944-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8944-123">Request headers</span></span>

| <span data-ttu-id="f8944-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f8944-124">Name</span></span>          | <span data-ttu-id="f8944-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8944-125">Type</span></span>   | <span data-ttu-id="f8944-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8944-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f8944-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8944-127">Authorization</span></span> | <span data-ttu-id="f8944-128">string</span><span class="sxs-lookup"><span data-stu-id="f8944-128">string</span></span> | <span data-ttu-id="f8944-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8944-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8944-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8944-131">Request body</span></span>

<span data-ttu-id="f8944-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8944-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8944-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f8944-133">Parameter</span></span>           | <span data-ttu-id="f8944-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8944-134">Type</span></span>    | <span data-ttu-id="f8944-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8944-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="f8944-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f8944-136">securityEnabledOnly</span></span> | <span data-ttu-id="f8944-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8944-137">Boolean</span></span> | <span data-ttu-id="f8944-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="f8944-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="f8944-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8944-140">Response</span></span>

<span data-ttu-id="f8944-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="f8944-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="f8944-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8944-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f8944-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8944-143">Request</span></span>

<span data-ttu-id="f8944-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8944-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f8944-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8944-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f8944-146">C#</span><span class="sxs-lookup"><span data-stu-id="f8944-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8944-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8944-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f8944-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8944-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f8944-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8944-149">Response</span></span>

<span data-ttu-id="f8944-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8944-150">The following is an example of the response.</span></span>

> <span data-ttu-id="f8944-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8944-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
