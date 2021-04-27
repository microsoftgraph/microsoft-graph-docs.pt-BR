---
title: Obter grupos de membros
description: Retorne todos os grupos dos qual o usuário, grupo, entidade de serviço ou objeto de diretório especificado é membro. Esta função é transitiva.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5813871a262475e85df93cfe82e6943f381f85b8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046850"
---
# <a name="get-member-groups"></a><span data-ttu-id="f6143-104">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="f6143-104">Get member groups</span></span>

<span data-ttu-id="f6143-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6143-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6143-106">Retorne todos os grupos dos qual o usuário, grupo, entidade de serviço ou objeto de diretório especificado é membro.</span><span class="sxs-lookup"><span data-stu-id="f6143-106">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="f6143-107">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="f6143-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6143-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6143-108">Permissions</span></span>
<span data-ttu-id="f6143-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6143-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6143-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6143-111">Permission type</span></span>      | <span data-ttu-id="f6143-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6143-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6143-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6143-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f6143-114">User.ReadBasic.All e GroupMember.Read.All, User.Read.All e GroupMember.Read.All, User.ReadBasic.All e Group.Read.All, User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6143-114">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="f6143-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6143-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6143-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6143-116">Not supported.</span></span>    |
|<span data-ttu-id="f6143-117">Application</span><span class="sxs-lookup"><span data-stu-id="f6143-117">Application</span></span> | <span data-ttu-id="f6143-118">User.Read.All e GroupMember.Read.All, User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6143-118">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="f6143-119">Use as diretrizes de cenário a seguir para ajudar a determinar quais tipos de permissão usar:</span><span class="sxs-lookup"><span data-stu-id="f6143-119">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="f6143-120">Use as permissões User.Read e GroupMember.Read.All ou User.Read e Group.Read.All para obter associações de grupo para o usuário associado.</span><span class="sxs-lookup"><span data-stu-id="f6143-120">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="f6143-121">Use User.ReadBasic.All e GroupMember.Read.All, User.Read.All e GroupMember.Read.All, User.ReadBasic.All e Group.Read.All ou User.Read.All e Group.Read.All para obter associações de grupo para qualquer usuário.</span><span class="sxs-lookup"><span data-stu-id="f6143-121">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="f6143-122">Use a permissão GroupMember.Read.All ou Group.Read.All para obter associações de grupo para um grupo.</span><span class="sxs-lookup"><span data-stu-id="f6143-122">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="f6143-123">Use as permissões Application.ReadWrite.All e GroupMember.Read.All ou Application.ReadWrite.All e Group.Read.All para obter associações de grupo para uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="f6143-123">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="f6143-124">Use a permissão Directory.Read.All para obter associações de grupo para um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="f6143-124">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="f6143-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6143-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="f6143-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6143-126">Request headers</span></span>
| <span data-ttu-id="f6143-127">Nome</span><span class="sxs-lookup"><span data-stu-id="f6143-127">Name</span></span>       | <span data-ttu-id="f6143-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6143-128">Type</span></span> | <span data-ttu-id="f6143-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6143-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6143-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6143-130">Authorization</span></span>  | <span data-ttu-id="f6143-131">string</span><span class="sxs-lookup"><span data-stu-id="f6143-131">string</span></span>  | <span data-ttu-id="f6143-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6143-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6143-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6143-134">Content-Type</span></span>  | <span data-ttu-id="f6143-135">application/json</span><span class="sxs-lookup"><span data-stu-id="f6143-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6143-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6143-136">Request body</span></span>
<span data-ttu-id="f6143-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6143-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f6143-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f6143-138">Parameter</span></span>    | <span data-ttu-id="f6143-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6143-139">Type</span></span>   |<span data-ttu-id="f6143-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6143-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6143-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f6143-141">securityEnabledOnly</span></span>|<span data-ttu-id="f6143-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6143-142">Boolean</span></span>| <span data-ttu-id="f6143-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="f6143-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="f6143-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6143-145">Response</span></span>

<span data-ttu-id="f6143-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6143-146">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6143-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6143-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f6143-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6143-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f6143-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6143-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="f6143-150">C#</span><span class="sxs-lookup"><span data-stu-id="f6143-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6143-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6143-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6143-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6143-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6143-153">Java</span><span class="sxs-lookup"><span data-stu-id="f6143-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6143-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6143-154">Response</span></span>
<span data-ttu-id="f6143-155">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f6143-155">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


