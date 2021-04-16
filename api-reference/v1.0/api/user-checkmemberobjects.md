---
title: 'user: checkMemberObjects'
description: Verifique se há associação em uma lista de funções de grupo ou diretório para o objeto de usuário especificado.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: df3cf26e98f3769bea4ceba632dccd24030494b0
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870062"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="b5894-103">user: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b5894-103">user: checkMemberObjects</span></span>

<span data-ttu-id="b5894-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5894-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5894-105">Verifique se há associação em uma lista de funções de grupo ou diretório para o objeto de usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="b5894-105">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="b5894-106">Esse método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="b5894-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5894-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5894-107">Permissions</span></span>

<span data-ttu-id="b5894-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5894-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5894-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5894-110">Permission type</span></span>                        | <span data-ttu-id="b5894-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5894-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5894-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5894-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5894-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5894-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="b5894-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5894-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5894-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5894-115">Not supported.</span></span> |
| <span data-ttu-id="b5894-116">Application</span><span class="sxs-lookup"><span data-stu-id="b5894-116">Application</span></span>                            | <span data-ttu-id="b5894-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5894-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5894-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5894-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="b5894-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5894-119">Request headers</span></span>

| <span data-ttu-id="b5894-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b5894-120">Name</span></span>          | <span data-ttu-id="b5894-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5894-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b5894-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5894-122">Authorization</span></span> | <span data-ttu-id="b5894-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5894-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5894-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5894-125">Content-Type</span></span>  | <span data-ttu-id="b5894-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5894-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5894-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5894-128">Request body</span></span>

<span data-ttu-id="b5894-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5894-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b5894-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b5894-130">Parameter</span></span>    | <span data-ttu-id="b5894-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5894-131">Type</span></span>        | <span data-ttu-id="b5894-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5894-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5894-133">ids</span><span class="sxs-lookup"><span data-stu-id="b5894-133">ids</span></span>|<span data-ttu-id="b5894-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5894-134">String collection</span></span>|<span data-ttu-id="b5894-135">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório ou IDs de roleTemplate de funções de diretório, na qual verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="b5894-135">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="b5894-136">Você pode especificar até 20 objetos.</span><span class="sxs-lookup"><span data-stu-id="b5894-136">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="b5894-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5894-137">Response</span></span>

<span data-ttu-id="b5894-138">Se tiver êxito, este método retornará um código de resposta e um novo objeto da coleção `200 OK` String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5894-138">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5894-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b5894-139">Examples</span></span>

<span data-ttu-id="b5894-140">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b5894-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b5894-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5894-141">Request</span></span>

<span data-ttu-id="b5894-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5894-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5894-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5894-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="b5894-144">C#</span><span class="sxs-lookup"><span data-stu-id="b5894-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5894-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5894-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5894-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5894-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5894-147">Java</span><span class="sxs-lookup"><span data-stu-id="b5894-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5894-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5894-148">Response</span></span>

<span data-ttu-id="b5894-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5894-149">The following is an example of the response.</span></span> 

><span data-ttu-id="b5894-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5894-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

