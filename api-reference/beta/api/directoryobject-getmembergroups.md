---
title: Obter grupos de membros
description: Retornar todos os grupos dos quais o usuário, grupo, entidade de serviço ou objeto de diretório especificado é um membro. Esta função é transitiva.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 847d3978aa346752d949cc5e82f390827d7639b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957784"
---
# <a name="get-member-groups"></a><span data-ttu-id="3e3db-104">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="3e3db-104">Get member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e3db-105">Retornar todos os grupos dos quais o usuário, grupo, entidade de serviço ou objeto de diretório especificado é um membro.</span><span class="sxs-lookup"><span data-stu-id="3e3db-105">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="3e3db-106">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="3e3db-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e3db-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e3db-107">Permissions</span></span>
<span data-ttu-id="3e3db-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e3db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3e3db-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e3db-110">Permission type</span></span>      | <span data-ttu-id="3e3db-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e3db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e3db-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e3db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e3db-113">User. ReadBasic. All e Group. Read. All, User. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="3e3db-113">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="3e3db-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e3db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e3db-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e3db-115">Not supported.</span></span>    |
|<span data-ttu-id="3e3db-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e3db-116">Application</span></span> | <span data-ttu-id="3e3db-117">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e3db-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="3e3db-118">Use as orientações de cenário a seguir para ajudar a determinar quais tipos de permissão usar:</span><span class="sxs-lookup"><span data-stu-id="3e3db-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="3e3db-119">Use as permissões User. Read e Group. Read. All para obter associações de grupo para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3e3db-119">Use User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="3e3db-120">Use as permissões User. ReadBasic. All e Group. Read. All ou User. Read. All e Group. Read. All para obter associações de grupo para qualquer usuário.</span><span class="sxs-lookup"><span data-stu-id="3e3db-120">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="3e3db-121">Use a permissão Group. Read. All para obter associações de grupo para um grupo.</span><span class="sxs-lookup"><span data-stu-id="3e3db-121">Use Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="3e3db-122">Use as permissões Application. ReadWrite. All e Group. Read. All para obter associações de grupo para uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="3e3db-122">Use Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="3e3db-123">Use a permissão Directory. Read. All para obter associações de grupo para um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="3e3db-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e3db-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e3db-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="3e3db-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e3db-125">Request headers</span></span>
| <span data-ttu-id="3e3db-126">Nome</span><span class="sxs-lookup"><span data-stu-id="3e3db-126">Name</span></span>       | <span data-ttu-id="3e3db-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e3db-127">Type</span></span> | <span data-ttu-id="3e3db-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e3db-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e3db-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e3db-129">Authorization</span></span>  | <span data-ttu-id="3e3db-130">string</span><span class="sxs-lookup"><span data-stu-id="3e3db-130">string</span></span>  | <span data-ttu-id="3e3db-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e3db-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e3db-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e3db-133">Content-Type</span></span>  | <span data-ttu-id="3e3db-134">application/json</span><span class="sxs-lookup"><span data-stu-id="3e3db-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e3db-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e3db-135">Request body</span></span>
<span data-ttu-id="3e3db-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e3db-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e3db-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3e3db-137">Parameter</span></span>    | <span data-ttu-id="3e3db-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e3db-138">Type</span></span>   |<span data-ttu-id="3e3db-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e3db-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e3db-140">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="3e3db-140">securityEnabledOnly</span></span>|<span data-ttu-id="3e3db-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e3db-141">Boolean</span></span>| <span data-ttu-id="3e3db-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="3e3db-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="3e3db-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e3db-144">Response</span></span>

<span data-ttu-id="3e3db-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e3db-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e3db-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e3db-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3e3db-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e3db-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3e3db-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e3db-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e3db-149">C#</span><span class="sxs-lookup"><span data-stu-id="3e3db-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e3db-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e3db-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e3db-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3e3db-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3e3db-152">Java</span><span class="sxs-lookup"><span data-stu-id="3e3db-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3e3db-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e3db-153">Response</span></span>
<span data-ttu-id="3e3db-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e3db-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
