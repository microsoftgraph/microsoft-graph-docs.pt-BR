---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação, que retorna somente os grupos dos quais o grupo é membro direto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e5b1d23ebce82770e218af0a3b4758b9ff86b07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953854"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="97dbc-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="97dbc-104">group: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97dbc-p102">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group-list-memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="97dbc-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="97dbc-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="97dbc-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="97dbc-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="97dbc-111">Permissions</span></span>

<span data-ttu-id="97dbc-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97dbc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97dbc-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97dbc-114">Permission type</span></span>                        | <span data-ttu-id="97dbc-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97dbc-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="97dbc-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97dbc-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="97dbc-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97dbc-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="97dbc-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97dbc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97dbc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97dbc-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="97dbc-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97dbc-120">Application</span></span>                            | <span data-ttu-id="97dbc-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97dbc-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="97dbc-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97dbc-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="97dbc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97dbc-123">Request headers</span></span>

| <span data-ttu-id="97dbc-124">Nome</span><span class="sxs-lookup"><span data-stu-id="97dbc-124">Name</span></span>          | <span data-ttu-id="97dbc-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="97dbc-125">Type</span></span>   | <span data-ttu-id="97dbc-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="97dbc-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="97dbc-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="97dbc-127">Authorization</span></span> | <span data-ttu-id="97dbc-128">string</span><span class="sxs-lookup"><span data-stu-id="97dbc-128">string</span></span> | <span data-ttu-id="97dbc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97dbc-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97dbc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97dbc-131">Request body</span></span>

<span data-ttu-id="97dbc-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97dbc-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="97dbc-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="97dbc-133">Parameter</span></span>           | <span data-ttu-id="97dbc-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="97dbc-134">Type</span></span>    | <span data-ttu-id="97dbc-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="97dbc-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="97dbc-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="97dbc-136">securityEnabledOnly</span></span> | <span data-ttu-id="97dbc-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="97dbc-137">Boolean</span></span> | <span data-ttu-id="97dbc-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="97dbc-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="97dbc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="97dbc-140">Response</span></span>

<span data-ttu-id="97dbc-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="97dbc-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="97dbc-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97dbc-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="97dbc-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97dbc-143">Request</span></span>

<span data-ttu-id="97dbc-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97dbc-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="97dbc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="97dbc-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="97dbc-146">C#</span><span class="sxs-lookup"><span data-stu-id="97dbc-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97dbc-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="97dbc-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97dbc-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="97dbc-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97dbc-149">Java</span><span class="sxs-lookup"><span data-stu-id="97dbc-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97dbc-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="97dbc-150">Response</span></span>

<span data-ttu-id="97dbc-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97dbc-151">The following is an example of the response.</span></span>

> <span data-ttu-id="97dbc-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97dbc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
