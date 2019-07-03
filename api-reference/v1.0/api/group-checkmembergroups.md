---
title: 'group: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: ad182a184455872b961af8f1df825774e29009db
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448142"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="61115-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="61115-104">group: checkMemberGroups</span></span>

<span data-ttu-id="61115-p102">Verifique se há associação na lista de grupos especificada. Retorna os grupos da lista com os quais o grupo especificado tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="61115-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="61115-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="61115-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="61115-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="61115-111">Permissions</span></span>

<span data-ttu-id="61115-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61115-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61115-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61115-114">Permission type</span></span>                        | <span data-ttu-id="61115-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61115-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="61115-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61115-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="61115-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61115-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="61115-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61115-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61115-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61115-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="61115-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61115-120">Application</span></span>                            | <span data-ttu-id="61115-121">Group. Read. All, Directory. Read. All.</span><span class="sxs-lookup"><span data-stu-id="61115-121">Group.Read.All, Directory.Read.All.</span></span> <span data-ttu-id="61115-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61115-122">Directory.ReadWrite.All</span></span>                               |



## <a name="http-request"></a><span data-ttu-id="61115-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61115-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="61115-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61115-124">Request headers</span></span>

| <span data-ttu-id="61115-125">Nome</span><span class="sxs-lookup"><span data-stu-id="61115-125">Name</span></span>          | <span data-ttu-id="61115-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="61115-126">Type</span></span>   | <span data-ttu-id="61115-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="61115-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="61115-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="61115-128">Authorization</span></span> | <span data-ttu-id="61115-129">string</span><span class="sxs-lookup"><span data-stu-id="61115-129">string</span></span> | <span data-ttu-id="61115-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61115-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61115-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61115-132">Request body</span></span>

<span data-ttu-id="61115-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61115-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="61115-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="61115-134">Parameter</span></span> | <span data-ttu-id="61115-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="61115-135">Type</span></span>              | <span data-ttu-id="61115-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="61115-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="61115-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="61115-137">groupIds</span></span>  | <span data-ttu-id="61115-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="61115-138">String collection</span></span> | <span data-ttu-id="61115-139">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="61115-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="61115-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="61115-140">Response</span></span>

<span data-ttu-id="61115-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61115-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61115-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61115-142">Example</span></span>

<span data-ttu-id="61115-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="61115-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="61115-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61115-144">Request</span></span>

<span data-ttu-id="61115-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61115-145">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="61115-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="61115-146">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="61115-147">C#</span><span class="sxs-lookup"><span data-stu-id="61115-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61115-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="61115-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61115-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61115-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="61115-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="61115-150">Response</span></span>

<span data-ttu-id="61115-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61115-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
