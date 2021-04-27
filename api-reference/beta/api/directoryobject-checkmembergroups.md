---
title: Verificar grupos de membros
description: Verifique se há associação em uma lista especificada de grupos e retorna dessa lista esses grupos
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0b52e42e3c610bf0f0020a2587ac7b649fc180be
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046878"
---
# <a name="check-member-groups"></a><span data-ttu-id="86a22-103">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="86a22-103">Check member groups</span></span>

<span data-ttu-id="86a22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a22-105">Verifique se há associação em uma lista especificada de grupos e retorna dessa lista os grupos dos quais o usuário, grupo, entidade de serviço ou objeto de diretório especificado é um membro.</span><span class="sxs-lookup"><span data-stu-id="86a22-105">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="86a22-106">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="86a22-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="86a22-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="86a22-107">Permissions</span></span>
<span data-ttu-id="86a22-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="86a22-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86a22-110">Permission type</span></span>      | <span data-ttu-id="86a22-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86a22-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86a22-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86a22-112">Delegated (work or school account)</span></span> | <span data-ttu-id="86a22-113">User.ReadBasic.All, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a22-113">User.ReadBasic.All, User.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="86a22-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86a22-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86a22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a22-115">Not supported.</span></span>    |
|<span data-ttu-id="86a22-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86a22-116">Application</span></span> | <span data-ttu-id="86a22-117">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a22-117">User.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="86a22-118">Use as diretrizes de cenário a seguir para ajudar a determinar quais tipos de permissão usar:</span><span class="sxs-lookup"><span data-stu-id="86a22-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="86a22-119">Use as permissões User.Read e GroupMember.Read.All ou User.Read e Group.Read.All para obter associações de grupo para o usuário associado.</span><span class="sxs-lookup"><span data-stu-id="86a22-119">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="86a22-120">Use User.ReadBasic.All e GroupMember.Read.All, User.Read.All e GroupMember.Read.All, User.ReadBasic.All e Group.Read.All ou User.Read.All e Group.Read.All para obter associações de grupo para qualquer usuário.</span><span class="sxs-lookup"><span data-stu-id="86a22-120">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="86a22-121">Use a permissão GroupMember.Read.All ou Group.Read.All para obter associações de grupo para um grupo.</span><span class="sxs-lookup"><span data-stu-id="86a22-121">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="86a22-122">Use as permissões Application.ReadWrite.All e GroupMember.Read.All ou Application.ReadWrite.All e Group.Read.All para obter associações de grupo para uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="86a22-122">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="86a22-123">Use a permissão Directory.Read.All para obter associações de grupo para um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="86a22-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="86a22-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86a22-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servicePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="86a22-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86a22-125">Request headers</span></span>
| <span data-ttu-id="86a22-126">Nome</span><span class="sxs-lookup"><span data-stu-id="86a22-126">Name</span></span>       | <span data-ttu-id="86a22-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="86a22-127">Type</span></span> | <span data-ttu-id="86a22-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a22-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86a22-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="86a22-129">Authorization</span></span>  | <span data-ttu-id="86a22-130">string</span><span class="sxs-lookup"><span data-stu-id="86a22-130">string</span></span>  | <span data-ttu-id="86a22-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86a22-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86a22-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86a22-133">Content-Type</span></span>  | <span data-ttu-id="86a22-134">application/json</span><span class="sxs-lookup"><span data-stu-id="86a22-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86a22-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86a22-135">Request body</span></span>
<span data-ttu-id="86a22-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86a22-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="86a22-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="86a22-137">Parameter</span></span>    | <span data-ttu-id="86a22-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="86a22-138">Type</span></span>   |<span data-ttu-id="86a22-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a22-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86a22-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="86a22-140">groupIds</span></span>|<span data-ttu-id="86a22-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="86a22-141">String collection</span></span> |<span data-ttu-id="86a22-p104">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="86a22-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="86a22-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a22-144">Response</span></span>

<span data-ttu-id="86a22-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86a22-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a22-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86a22-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="86a22-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86a22-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="86a22-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="86a22-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="86a22-149">C#</span><span class="sxs-lookup"><span data-stu-id="86a22-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86a22-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86a22-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86a22-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86a22-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86a22-152">Java</span><span class="sxs-lookup"><span data-stu-id="86a22-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="86a22-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a22-153">Response</span></span>
<span data-ttu-id="86a22-154">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86a22-154">Note: The response object shown here might be shortened for readability.</span></span>
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


