---
title: 'group: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 9d76df33ac36ef936a1abfa873332c3be3aa0650
ms.sourcegitcommit: 6d8bf390380b9434ba626d6dc5101afcf6ba6f8b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2019
ms.locfileid: "35395181"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="0a1d1-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="0a1d1-104">group: checkMemberGroups</span></span>

<span data-ttu-id="0a1d1-p102">Verifique se há associação na lista de grupos especificada. Retorna os grupos da lista com os quais o grupo especificado tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="0a1d1-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a1d1-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a1d1-111">Permissions</span></span>

<span data-ttu-id="0a1d1-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a1d1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a1d1-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a1d1-114">Permission type</span></span>                        | <span data-ttu-id="0a1d1-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a1d1-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="0a1d1-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a1d1-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a1d1-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0a1d1-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="0a1d1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a1d1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a1d1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="0a1d1-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a1d1-120">Application</span></span>                            | <span data-ttu-id="0a1d1-121">Group. Read. All, Directory. Read. All.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-121">Group.Read.All, Directory.Read.All.</span></span> <span data-ttu-id="0a1d1-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a1d1-122">Directory.ReadWrite.All</span></span>                               |



## <a name="http-request"></a><span data-ttu-id="0a1d1-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1d1-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="0a1d1-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1d1-124">Request headers</span></span>

| <span data-ttu-id="0a1d1-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0a1d1-125">Name</span></span>          | <span data-ttu-id="0a1d1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a1d1-126">Type</span></span>   | <span data-ttu-id="0a1d1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a1d1-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="0a1d1-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a1d1-128">Authorization</span></span> | <span data-ttu-id="0a1d1-129">string</span><span class="sxs-lookup"><span data-stu-id="0a1d1-129">string</span></span> | <span data-ttu-id="0a1d1-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a1d1-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1d1-132">Request body</span></span>

<span data-ttu-id="0a1d1-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0a1d1-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0a1d1-134">Parameter</span></span> | <span data-ttu-id="0a1d1-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a1d1-135">Type</span></span>              | <span data-ttu-id="0a1d1-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a1d1-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="0a1d1-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="0a1d1-137">groupIds</span></span>  | <span data-ttu-id="0a1d1-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1d1-138">String collection</span></span> | <span data-ttu-id="0a1d1-139">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="0a1d1-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="0a1d1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1d1-140">Response</span></span>

<span data-ttu-id="0a1d1-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1d1-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a1d1-142">Example</span></span>

<span data-ttu-id="0a1d1-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0a1d1-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1d1-144">Request</span></span>

<span data-ttu-id="0a1d1-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="0a1d1-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1d1-146">Response</span></span>

<span data-ttu-id="0a1d1-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a1d1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a1d1-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0a1d1-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a1d1-151">C#</span><span class="sxs-lookup"><span data-stu-id="0a1d1-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a1d1-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a1d1-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0a1d1-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a1d1-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
