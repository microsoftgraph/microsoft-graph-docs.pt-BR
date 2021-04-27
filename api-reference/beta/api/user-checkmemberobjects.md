---
title: 'user: checkMemberObjects'
description: Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa para o objeto de usuário especificado.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 82ba7a3ca85f940d15dc0e16542f3129d79c2bc0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053381"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="a0bd4-103">user: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a0bd4-103">user: checkMemberObjects</span></span>

<span data-ttu-id="a0bd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0bd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0bd4-105">Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa para o objeto de usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-105">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="a0bd4-106">Esse método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0bd4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0bd4-107">Permissions</span></span>

<span data-ttu-id="a0bd4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0bd4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0bd4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0bd4-110">Permission type</span></span>                        | <span data-ttu-id="a0bd4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0bd4-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0bd4-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0bd4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0bd4-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0bd4-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="a0bd4-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0bd4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0bd4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-115">Not supported.</span></span> |
| <span data-ttu-id="a0bd4-116">Application</span><span class="sxs-lookup"><span data-stu-id="a0bd4-116">Application</span></span>                            | <span data-ttu-id="a0bd4-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0bd4-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0bd4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0bd4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="a0bd4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bd4-119">Request headers</span></span>

| <span data-ttu-id="a0bd4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a0bd4-120">Name</span></span>          | <span data-ttu-id="a0bd4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0bd4-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a0bd4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0bd4-122">Authorization</span></span> | <span data-ttu-id="a0bd4-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a0bd4-123">Bearer {token}</span></span> |
| <span data-ttu-id="a0bd4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0bd4-124">Content-Type</span></span>  | <span data-ttu-id="a0bd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0bd4-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0bd4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bd4-126">Request body</span></span>

<span data-ttu-id="a0bd4-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a0bd4-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a0bd4-128">Parameter</span></span>    | <span data-ttu-id="a0bd4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0bd4-129">Type</span></span>        | <span data-ttu-id="a0bd4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0bd4-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0bd4-131">ids</span><span class="sxs-lookup"><span data-stu-id="a0bd4-131">ids</span></span>|<span data-ttu-id="a0bd4-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0bd4-132">String collection</span></span>|<span data-ttu-id="a0bd4-133">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs de roleTemplate de funções de diretório, na qual verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="a0bd4-134">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-134">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="a0bd4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bd4-135">Response</span></span>

<span data-ttu-id="a0bd4-136">Se tiver êxito, este método retornará um código de resposta e um novo objeto da coleção `200 OK` String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-136">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0bd4-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0bd4-137">Examples</span></span>

<span data-ttu-id="a0bd4-138">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-138">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a0bd4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bd4-139">Request</span></span>

<span data-ttu-id="a0bd4-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0bd4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0bd4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="a0bd4-142">C#</span><span class="sxs-lookup"><span data-stu-id="a0bd4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0bd4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0bd4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0bd4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0bd4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0bd4-145">Java</span><span class="sxs-lookup"><span data-stu-id="a0bd4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0bd4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bd4-146">Response</span></span>

<span data-ttu-id="a0bd4-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-147">The following is an example of the response.</span></span> 

><span data-ttu-id="a0bd4-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a0bd4-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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


