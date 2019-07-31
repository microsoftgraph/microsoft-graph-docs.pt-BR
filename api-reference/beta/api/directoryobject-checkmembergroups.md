---
title: Verificar grupos de membros
description: Verificar se há associação em uma lista de grupos especificada e retorna dessa lista esses grupos
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 471435b7ff0ea7dc9bfcdba82db41772a3945b53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951225"
---
# <a name="check-member-groups"></a><span data-ttu-id="13654-103">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="13654-103">Check member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13654-104">Verifique se há associação em uma lista especificada de grupos e retorna dessa lista os grupos dos quais o usuário, grupo, entidade de serviço ou objeto de diretório especificado é um membro.</span><span class="sxs-lookup"><span data-stu-id="13654-104">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="13654-105">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="13654-105">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="13654-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13654-106">Permissions</span></span>
<span data-ttu-id="13654-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13654-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="13654-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13654-109">Permission type</span></span>      | <span data-ttu-id="13654-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13654-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13654-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13654-111">Delegated (work or school account)</span></span> | <span data-ttu-id="13654-112">User. ReadBasic. All e Group. Read. All, User. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="13654-112">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="13654-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13654-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13654-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13654-114">Not supported.</span></span>    |
|<span data-ttu-id="13654-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13654-115">Application</span></span> | <span data-ttu-id="13654-116">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="13654-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="13654-117">Use as orientações de cenário a seguir para ajudar a determinar quais tipos de permissão usar:</span><span class="sxs-lookup"><span data-stu-id="13654-117">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="13654-118">Use as permissões User. Read e Group. Read. All para verificar as associações de grupo para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="13654-118">Use User.Read and Group.Read.All permissions to check group memberships for the signed-in user.</span></span>
- <span data-ttu-id="13654-119">Use as permissões User. ReadBasic. All e Group. Read. All ou User. Read. All e Group. Read. All para verificar as associações de grupo para qualquer usuário.</span><span class="sxs-lookup"><span data-stu-id="13654-119">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to check group memberships for any user.</span></span>
- <span data-ttu-id="13654-120">Use a permissão Group. Read. All para verificar os membros do grupo para um grupo.</span><span class="sxs-lookup"><span data-stu-id="13654-120">Use Group.Read.All permission to check group memberships for a group.</span></span>
- <span data-ttu-id="13654-121">Use as permissões Application. ReadWrite. All e Group. Read. All para verificar as associações de grupo para uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="13654-121">Use Application.ReadWrite.All and Group.Read.All permissions to check group memberships for a service principal.</span></span>
- <span data-ttu-id="13654-122">Use a permissão Directory. Read. All para verificar as associações de grupo para um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="13654-122">Use Directory.Read.All permission to check group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="13654-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13654-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servicePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="13654-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13654-124">Request headers</span></span>
| <span data-ttu-id="13654-125">Nome</span><span class="sxs-lookup"><span data-stu-id="13654-125">Name</span></span>       | <span data-ttu-id="13654-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="13654-126">Type</span></span> | <span data-ttu-id="13654-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="13654-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13654-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="13654-128">Authorization</span></span>  | <span data-ttu-id="13654-129">string</span><span class="sxs-lookup"><span data-stu-id="13654-129">string</span></span>  | <span data-ttu-id="13654-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13654-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13654-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13654-132">Content-Type</span></span>  | <span data-ttu-id="13654-133">application/json</span><span class="sxs-lookup"><span data-stu-id="13654-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13654-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13654-134">Request body</span></span>
<span data-ttu-id="13654-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13654-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="13654-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="13654-136">Parameter</span></span>    | <span data-ttu-id="13654-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="13654-137">Type</span></span>   |<span data-ttu-id="13654-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="13654-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13654-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="13654-139">groupIds</span></span>|<span data-ttu-id="13654-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="13654-140">String collection</span></span> |<span data-ttu-id="13654-p104">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="13654-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="13654-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="13654-143">Response</span></span>

<span data-ttu-id="13654-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13654-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13654-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13654-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="13654-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13654-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="13654-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="13654-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="13654-148">C#</span><span class="sxs-lookup"><span data-stu-id="13654-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13654-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="13654-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13654-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="13654-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="13654-151">Java</span><span class="sxs-lookup"><span data-stu-id="13654-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="13654-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="13654-152">Response</span></span>
<span data-ttu-id="13654-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13654-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
