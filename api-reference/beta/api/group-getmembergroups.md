---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação, que retorna somente os grupos dos quais o grupo é membro direto.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1e677d3aa033283417bfe6292d801455b425dff6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895843"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="f9eb6-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f9eb6-104">group: getMemberGroups</span></span>

<span data-ttu-id="f9eb6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9eb6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9eb6-106">Return all the groups that the specified group is a member of.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-106">Return all the groups that the specified group is a member of.</span></span> <span data-ttu-id="f9eb6-107">The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-107">The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="f9eb6-108">Essa função suporta o Microsoft 365 e outros tipos de grupos provisionados no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="f9eb6-109">O número máximo de grupos que cada solicitação pode retornar é 2046.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-109">The maximum number of groups each request can return is 2046.</span></span> <span data-ttu-id="f9eb6-110">Observe que os grupos do Microsoft 365 não podem conter grupos.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-110">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="f9eb6-111">Portanto, a associação a um grupo do Microsoft 365 é sempre direta.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-111">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9eb6-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9eb6-112">Permissions</span></span>

<span data-ttu-id="f9eb6-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f9eb6-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9eb6-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9eb6-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9eb6-115">Permission type</span></span>                        | <span data-ttu-id="f9eb6-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9eb6-116">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="f9eb6-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9eb6-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9eb6-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9eb6-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f9eb6-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9eb6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9eb6-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-120">Not supported.</span></span>                                                                              |
| <span data-ttu-id="f9eb6-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9eb6-121">Application</span></span>                            | <span data-ttu-id="f9eb6-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9eb6-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="f9eb6-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9eb6-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="f9eb6-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9eb6-124">Request headers</span></span>

| <span data-ttu-id="f9eb6-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f9eb6-125">Name</span></span>          | <span data-ttu-id="f9eb6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9eb6-126">Type</span></span>   | <span data-ttu-id="f9eb6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9eb6-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f9eb6-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9eb6-128">Authorization</span></span> | <span data-ttu-id="f9eb6-129">string</span><span class="sxs-lookup"><span data-stu-id="f9eb6-129">string</span></span> | <span data-ttu-id="f9eb6-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-130">Bearer {token}.</span></span> <span data-ttu-id="f9eb6-131">Required.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9eb6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9eb6-132">Request body</span></span>

<span data-ttu-id="f9eb6-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9eb6-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f9eb6-134">Parameter</span></span>           | <span data-ttu-id="f9eb6-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9eb6-135">Type</span></span>    | <span data-ttu-id="f9eb6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9eb6-136">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="f9eb6-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f9eb6-137">securityEnabledOnly</span></span> | <span data-ttu-id="f9eb6-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9eb6-138">Boolean</span></span> | <span data-ttu-id="f9eb6-139">Set to **false**.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-139">Set to **false**.</span></span> <span data-ttu-id="f9eb6-140">Returning only security-enabled groups is supported for users only.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-140">Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="f9eb6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9eb6-141">Response</span></span>

<span data-ttu-id="f9eb6-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="f9eb6-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9eb6-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f9eb6-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9eb6-144">Request</span></span>

<span data-ttu-id="f9eb6-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f9eb6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9eb6-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f9eb6-147">C#</span><span class="sxs-lookup"><span data-stu-id="f9eb6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9eb6-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9eb6-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9eb6-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9eb6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f9eb6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9eb6-150">Response</span></span>

<span data-ttu-id="f9eb6-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-151">The following is an example of the response.</span></span>

> <span data-ttu-id="f9eb6-152">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f9eb6-153">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f9eb6-153">All the properties will be returned from an actual call.</span></span>

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
