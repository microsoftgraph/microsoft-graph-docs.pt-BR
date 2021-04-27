---
title: 'group: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 49830cfd8669ea44ac386bdc394e5582e5e5e3d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042146"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="78309-103">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="78309-103">group: checkMemberGroups</span></span>

<span data-ttu-id="78309-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78309-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78309-p101">Verifique se há associação na lista de grupos especificada. Retorna os grupos da lista com os quais o grupo especificado tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="78309-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="78309-p102">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Microsoft 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Microsoft 365 não podem conter grupos, então associações em um Grupo do Microsoft 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="78309-p102">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="78309-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="78309-111">Permissions</span></span>

<span data-ttu-id="78309-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78309-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78309-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78309-114">Permission type</span></span>                        | <span data-ttu-id="78309-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78309-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="78309-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78309-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="78309-117">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="78309-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="78309-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78309-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78309-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78309-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="78309-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78309-120">Application</span></span>                            | <span data-ttu-id="78309-121">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="78309-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="78309-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78309-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="78309-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78309-123">Request headers</span></span>

| <span data-ttu-id="78309-124">Nome</span><span class="sxs-lookup"><span data-stu-id="78309-124">Name</span></span>          | <span data-ttu-id="78309-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="78309-125">Type</span></span>   | <span data-ttu-id="78309-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="78309-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="78309-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="78309-127">Authorization</span></span> | <span data-ttu-id="78309-128">string</span><span class="sxs-lookup"><span data-stu-id="78309-128">string</span></span> | <span data-ttu-id="78309-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78309-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78309-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78309-131">Request body</span></span>

<span data-ttu-id="78309-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78309-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78309-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="78309-133">Parameter</span></span> | <span data-ttu-id="78309-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="78309-134">Type</span></span>   | <span data-ttu-id="78309-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="78309-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="78309-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="78309-136">groupIds</span></span>  | <span data-ttu-id="78309-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="78309-137">String collection</span></span> | <span data-ttu-id="78309-138">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="78309-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="78309-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="78309-139">Response</span></span>

<span data-ttu-id="78309-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78309-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78309-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78309-141">Example</span></span>

<span data-ttu-id="78309-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="78309-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="78309-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78309-143">Request</span></span>

<span data-ttu-id="78309-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78309-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="78309-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="78309-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="78309-146">C#</span><span class="sxs-lookup"><span data-stu-id="78309-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78309-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78309-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78309-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78309-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78309-149">Java</span><span class="sxs-lookup"><span data-stu-id="78309-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="78309-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="78309-150">Response</span></span>

<span data-ttu-id="78309-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78309-151">Here is an example of the response.</span></span> <span data-ttu-id="78309-152">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="78309-152">Note: The response object shown here might be shortened for readability.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


