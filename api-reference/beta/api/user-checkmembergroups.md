---
title: checkMemberGroups
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e5559e2c581e573e8154168ba5bd1db39cdb536e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896473"
---
# <a name="checkmembergroups"></a><span data-ttu-id="aef92-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="aef92-104">checkMemberGroups</span></span>

<span data-ttu-id="aef92-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aef92-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aef92-106">Check for membership in the specified list of groups.</span><span class="sxs-lookup"><span data-stu-id="aef92-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="aef92-107">Returns from the list those groups of which the user has a direct or transitive membership.</span><span class="sxs-lookup"><span data-stu-id="aef92-107">Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="aef92-108">You can check up to a maximum of 20 groups per request.</span><span class="sxs-lookup"><span data-stu-id="aef92-108">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="aef92-109">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aef92-109">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="aef92-110">Note that Microsoft 365 groups cannot contain groups.</span><span class="sxs-lookup"><span data-stu-id="aef92-110">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="aef92-111">So membership in a Microsoft 365 group is always direct.</span><span class="sxs-lookup"><span data-stu-id="aef92-111">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="aef92-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="aef92-112">Permissions</span></span>

<span data-ttu-id="aef92-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="aef92-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="aef92-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef92-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aef92-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aef92-115">Permission type</span></span>                        | <span data-ttu-id="aef92-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aef92-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="aef92-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aef92-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="aef92-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aef92-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="aef92-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aef92-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aef92-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aef92-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="aef92-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aef92-121">Application</span></span>                            | <span data-ttu-id="aef92-122">User. Read. All e GroupMember. Read. All, User. Read. All e Group. Read. All, User. ReadWrite. All e GroupMember. Read. All, User. ReadWrite. All e Group. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aef92-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aef92-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aef92-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="aef92-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aef92-124">Request headers</span></span>

| <span data-ttu-id="aef92-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aef92-125">Header</span></span>        | <span data-ttu-id="aef92-126">Valor</span><span class="sxs-lookup"><span data-stu-id="aef92-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="aef92-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="aef92-127">Authorization</span></span> | <span data-ttu-id="aef92-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="aef92-128">Bearer {token}.</span></span> <span data-ttu-id="aef92-129">Required.</span><span class="sxs-lookup"><span data-stu-id="aef92-129">Required.</span></span> |
| <span data-ttu-id="aef92-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aef92-130">Content-Type</span></span>  | <span data-ttu-id="aef92-131">application/json</span><span class="sxs-lookup"><span data-stu-id="aef92-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="aef92-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aef92-132">Request body</span></span>

<span data-ttu-id="aef92-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aef92-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aef92-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aef92-134">Parameter</span></span> | <span data-ttu-id="aef92-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="aef92-135">Type</span></span>   | <span data-ttu-id="aef92-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="aef92-136">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="aef92-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="aef92-137">groupIds</span></span>  | <span data-ttu-id="aef92-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aef92-138">String collection</span></span> | <span data-ttu-id="aef92-139">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="aef92-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="aef92-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef92-140">Response</span></span>

<span data-ttu-id="aef92-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aef92-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aef92-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aef92-142">Example</span></span>

<span data-ttu-id="aef92-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="aef92-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="aef92-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aef92-144">Request</span></span>

<span data-ttu-id="aef92-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aef92-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aef92-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="aef92-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="aef92-147">C#</span><span class="sxs-lookup"><span data-stu-id="aef92-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aef92-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aef92-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aef92-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aef92-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aef92-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef92-150">Response</span></span>

<span data-ttu-id="aef92-151">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="aef92-151">Here is an example of the response.</span></span> <span data-ttu-id="aef92-152">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="aef92-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aef92-153">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="aef92-153">All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
