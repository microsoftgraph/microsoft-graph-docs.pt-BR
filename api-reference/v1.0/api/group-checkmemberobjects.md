---
title: 'group: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos ou funções de diretório para o objeto de grupo especificado.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 076fb6007d856d02f06eb874f0ea3e3f6e211a66
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870020"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="e9cbc-103">group: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e9cbc-103">group: checkMemberObjects</span></span>

<span data-ttu-id="e9cbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9cbc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9cbc-105">Verifique se há associação em uma lista de grupos ou funções de diretório para o grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-105">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="e9cbc-106">Esse método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9cbc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9cbc-107">Permissions</span></span>

<span data-ttu-id="e9cbc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9cbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9cbc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9cbc-110">Permission type</span></span>                        | <span data-ttu-id="e9cbc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9cbc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9cbc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9cbc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9cbc-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9cbc-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="e9cbc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9cbc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9cbc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-115">Not supported.</span></span> |
| <span data-ttu-id="e9cbc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9cbc-116">Application</span></span>                            | <span data-ttu-id="e9cbc-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9cbc-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9cbc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9cbc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="e9cbc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9cbc-119">Request headers</span></span>

| <span data-ttu-id="e9cbc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e9cbc-120">Name</span></span>          | <span data-ttu-id="e9cbc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9cbc-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e9cbc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9cbc-122">Authorization</span></span> | <span data-ttu-id="e9cbc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9cbc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9cbc-125">Content-Type</span></span>  | <span data-ttu-id="e9cbc-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9cbc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9cbc-128">Request body</span></span>

<span data-ttu-id="e9cbc-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9cbc-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e9cbc-130">Parameter</span></span>    | <span data-ttu-id="e9cbc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9cbc-131">Type</span></span>        | <span data-ttu-id="e9cbc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9cbc-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9cbc-133">ids</span><span class="sxs-lookup"><span data-stu-id="e9cbc-133">ids</span></span>|<span data-ttu-id="e9cbc-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9cbc-134">String collection</span></span>| <span data-ttu-id="e9cbc-135">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório ou IDs de roleTemplate de funções de diretório, na qual verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-135">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="e9cbc-136">Você pode especificar até 20 objetos.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-136">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="e9cbc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9cbc-137">Response</span></span>

<span data-ttu-id="e9cbc-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-138">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9cbc-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e9cbc-139">Examples</span></span>

<span data-ttu-id="e9cbc-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e9cbc-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9cbc-141">Request</span></span>

<span data-ttu-id="e9cbc-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9cbc-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9cbc-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="e9cbc-144">C#</span><span class="sxs-lookup"><span data-stu-id="e9cbc-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9cbc-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9cbc-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9cbc-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9cbc-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9cbc-147">Java</span><span class="sxs-lookup"><span data-stu-id="e9cbc-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9cbc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9cbc-148">Response</span></span>

<span data-ttu-id="e9cbc-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-149">The following is an example of the response.</span></span> 

> <span data-ttu-id="e9cbc-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9cbc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

