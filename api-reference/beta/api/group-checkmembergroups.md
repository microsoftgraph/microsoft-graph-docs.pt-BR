---
title: 'group: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9235d8b30801c32d2428f4086ab8ce22ed021fa3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895871"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="99955-103">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="99955-103">group: checkMemberGroups</span></span>

<span data-ttu-id="99955-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99955-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99955-105">Check for membership in the specified list of groups.</span><span class="sxs-lookup"><span data-stu-id="99955-105">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="99955-106">Returns from the list those groups of which the specified group has a direct or transitive membership.</span><span class="sxs-lookup"><span data-stu-id="99955-106">Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="99955-107">You can check up to a maximum of 20 groups per request.</span><span class="sxs-lookup"><span data-stu-id="99955-107">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="99955-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="99955-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="99955-109">Note that Microsoft 365 groups cannot contain groups.</span><span class="sxs-lookup"><span data-stu-id="99955-109">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="99955-110">So membership in a Microsoft 365 group is always direct.</span><span class="sxs-lookup"><span data-stu-id="99955-110">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="99955-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="99955-111">Permissions</span></span>

<span data-ttu-id="99955-112">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="99955-112">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="99955-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99955-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99955-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99955-114">Permission type</span></span>                        | <span data-ttu-id="99955-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99955-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="99955-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99955-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="99955-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="99955-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="99955-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99955-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99955-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99955-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="99955-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99955-120">Application</span></span>                            | <span data-ttu-id="99955-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99955-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="99955-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99955-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="99955-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99955-123">Request headers</span></span>

| <span data-ttu-id="99955-124">Nome</span><span class="sxs-lookup"><span data-stu-id="99955-124">Name</span></span>          | <span data-ttu-id="99955-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="99955-125">Type</span></span>   | <span data-ttu-id="99955-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="99955-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="99955-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="99955-127">Authorization</span></span> | <span data-ttu-id="99955-128">string</span><span class="sxs-lookup"><span data-stu-id="99955-128">string</span></span> | <span data-ttu-id="99955-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="99955-129">Bearer {token}.</span></span> <span data-ttu-id="99955-130">Required.</span><span class="sxs-lookup"><span data-stu-id="99955-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99955-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99955-131">Request body</span></span>

<span data-ttu-id="99955-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99955-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99955-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="99955-133">Parameter</span></span> | <span data-ttu-id="99955-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="99955-134">Type</span></span>   | <span data-ttu-id="99955-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="99955-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="99955-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="99955-136">groupIds</span></span>  | <span data-ttu-id="99955-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="99955-137">String collection</span></span> | <span data-ttu-id="99955-138">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="99955-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="99955-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="99955-139">Response</span></span>

<span data-ttu-id="99955-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99955-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99955-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99955-141">Example</span></span>

<span data-ttu-id="99955-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="99955-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="99955-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99955-143">Request</span></span>

<span data-ttu-id="99955-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99955-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="99955-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="99955-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="99955-146">C#</span><span class="sxs-lookup"><span data-stu-id="99955-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99955-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99955-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99955-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99955-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99955-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="99955-149">Response</span></span>

<span data-ttu-id="99955-150">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="99955-150">Here is an example of the response.</span></span> <span data-ttu-id="99955-151">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="99955-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99955-152">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="99955-152">All of the properties will be returned from an actual call.</span></span>

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
