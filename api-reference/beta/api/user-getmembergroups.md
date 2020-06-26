---
title: 'usuário: getMemberGroups'
description: Retorne todos os grupos dos quais o usuário é membro. A verificação foi transitiva, ao contrário de leitura a
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c2ab1bcd9dce8e933ed65d51dd9b0ce010bc1b90
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896466"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="11298-104">usuário: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="11298-104">user: getMemberGroups</span></span>

<span data-ttu-id="11298-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11298-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11298-106">Return all the groups that the user is a member of.</span><span class="sxs-lookup"><span data-stu-id="11298-106">Return all the groups that the user is a member of.</span></span> <span data-ttu-id="11298-107">The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span><span class="sxs-lookup"><span data-stu-id="11298-107">The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="11298-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="11298-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="11298-109">The maximum number of groups each request can return is 2046.</span><span class="sxs-lookup"><span data-stu-id="11298-109">The maximum number of groups each request can return is 2046.</span></span> <span data-ttu-id="11298-110">Note that Microsoft 365 groups cannot contain groups.</span><span class="sxs-lookup"><span data-stu-id="11298-110">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="11298-111">So membership in a Microsoft 365 group is always direct.</span><span class="sxs-lookup"><span data-stu-id="11298-111">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="11298-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="11298-112">Permissions</span></span>

<span data-ttu-id="11298-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="11298-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="11298-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11298-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11298-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11298-115">Permission type</span></span>                        | <span data-ttu-id="11298-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11298-116">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="11298-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11298-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="11298-118">User. ReadBasic. All e GroupMember. Read. All, User. Read e GroupMember. Read. All, User. Read. All e GroupMember. Read. All, User. ReadBasic. All e Group. Read. All, User. Read e Group. Read. All, User. Read. All e Group. Read. All, Directory. Read. All, Directory.. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="11298-118">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="11298-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11298-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11298-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11298-120">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="11298-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11298-121">Application</span></span>                            | <span data-ttu-id="11298-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11298-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>            |

## <a name="http-request"></a><span data-ttu-id="11298-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11298-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="11298-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11298-124">Request headers</span></span>

| <span data-ttu-id="11298-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11298-125">Header</span></span>        | <span data-ttu-id="11298-126">Valor</span><span class="sxs-lookup"><span data-stu-id="11298-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="11298-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="11298-127">Authorization</span></span> | <span data-ttu-id="11298-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="11298-128">Bearer {token}.</span></span> <span data-ttu-id="11298-129">Required.</span><span class="sxs-lookup"><span data-stu-id="11298-129">Required.</span></span> |
| <span data-ttu-id="11298-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11298-130">Content-Type</span></span>  | <span data-ttu-id="11298-131">application/json</span><span class="sxs-lookup"><span data-stu-id="11298-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="11298-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11298-132">Request body</span></span>

<span data-ttu-id="11298-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11298-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11298-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="11298-134">Parameter</span></span>           | <span data-ttu-id="11298-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="11298-135">Type</span></span>    | <span data-ttu-id="11298-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="11298-136">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="11298-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="11298-137">securityEnabledOnly</span></span> | <span data-ttu-id="11298-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="11298-138">Boolean</span></span> | <span data-ttu-id="11298-139">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned.</span><span class="sxs-lookup"><span data-stu-id="11298-139">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned.</span></span> <span data-ttu-id="11298-140">Note: Setting this parameter to **true** is only supported when calling this method on a user.</span><span class="sxs-lookup"><span data-stu-id="11298-140">Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="11298-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="11298-141">Response</span></span>

<span data-ttu-id="11298-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="11298-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="11298-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11298-143">Example</span></span>

<span data-ttu-id="11298-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="11298-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="11298-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11298-145">Request</span></span>

<span data-ttu-id="11298-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11298-146">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11298-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="11298-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="11298-148">C#</span><span class="sxs-lookup"><span data-stu-id="11298-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11298-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11298-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11298-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11298-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="11298-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="11298-151">Response</span></span>

<span data-ttu-id="11298-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="11298-152">Here is an example of the response.</span></span> <span data-ttu-id="11298-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="11298-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="11298-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="11298-154">All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
