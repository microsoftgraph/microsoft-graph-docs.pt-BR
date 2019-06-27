---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação, que retorna somente os grupos dos quais o grupo é membro direto.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8a3b2fa52ff12b30e431c5dc925dffd6090b31ac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273553"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="e6cca-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e6cca-104">group: getMemberGroups</span></span>

<span data-ttu-id="e6cca-p102">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group-list-memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="e6cca-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="e6cca-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="e6cca-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6cca-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6cca-111">Permissions</span></span>

<span data-ttu-id="e6cca-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6cca-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6cca-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6cca-114">Permission type</span></span>                        | <span data-ttu-id="e6cca-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6cca-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="e6cca-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6cca-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6cca-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6cca-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="e6cca-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6cca-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6cca-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6cca-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="e6cca-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6cca-120">Application</span></span>                            | <span data-ttu-id="e6cca-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6cca-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |


## <a name="http-request"></a><span data-ttu-id="e6cca-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6cca-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="e6cca-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cca-123">Request headers</span></span>

| <span data-ttu-id="e6cca-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e6cca-124">Name</span></span>          | <span data-ttu-id="e6cca-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6cca-125">Type</span></span>   | <span data-ttu-id="e6cca-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6cca-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="e6cca-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6cca-127">Authorization</span></span> | <span data-ttu-id="e6cca-128">string</span><span class="sxs-lookup"><span data-stu-id="e6cca-128">string</span></span> | <span data-ttu-id="e6cca-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6cca-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6cca-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cca-131">Request body</span></span>

<span data-ttu-id="e6cca-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6cca-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6cca-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6cca-133">Parameter</span></span>           | <span data-ttu-id="e6cca-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6cca-134">Type</span></span>    | <span data-ttu-id="e6cca-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6cca-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="e6cca-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e6cca-136">securityEnabledOnly</span></span> | <span data-ttu-id="e6cca-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6cca-137">Boolean</span></span> | <span data-ttu-id="e6cca-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="e6cca-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="e6cca-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6cca-140">Response</span></span>

<span data-ttu-id="e6cca-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="e6cca-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="e6cca-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6cca-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e6cca-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cca-143">Request</span></span>

<span data-ttu-id="e6cca-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6cca-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="e6cca-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6cca-145">Response</span></span>

<span data-ttu-id="e6cca-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6cca-146">The following is an example of the response.</span></span>

> <span data-ttu-id="e6cca-147">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e6cca-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e6cca-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6cca-148">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6cca-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e6cca-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6cca-150">C#</span><span class="sxs-lookup"><span data-stu-id="e6cca-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6cca-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6cca-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_getmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e6cca-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6cca-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_getmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
