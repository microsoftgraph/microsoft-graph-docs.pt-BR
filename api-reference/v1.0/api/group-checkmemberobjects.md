---
title: 'group: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos ou funções de diretório para o objeto de grupo especificado.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 35ad4cc491d0a3d8513ca070a258ecc8e6080e8f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135587"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="ef1af-103">group: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="ef1af-103">group: checkMemberObjects</span></span>

<span data-ttu-id="ef1af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef1af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef1af-105">Verifique se há associação em uma lista de grupos ou funções de diretório para o grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="ef1af-105">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="ef1af-106">Esse método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="ef1af-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef1af-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ef1af-107">Permissions</span></span>

<span data-ttu-id="ef1af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef1af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef1af-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef1af-110">Permission type</span></span>                        | <span data-ttu-id="ef1af-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef1af-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ef1af-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef1af-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef1af-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1af-113">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="ef1af-114">E:</span><span class="sxs-lookup"><span data-stu-id="ef1af-114">And:</span></span><br><ul><li><span data-ttu-id="ef1af-115">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1af-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="ef1af-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef1af-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ef1af-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef1af-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef1af-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef1af-118">Not supported.</span></span> |
| <span data-ttu-id="ef1af-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef1af-119">Application</span></span>                            | <span data-ttu-id="ef1af-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1af-120">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="ef1af-121">E:</span><span class="sxs-lookup"><span data-stu-id="ef1af-121">And:</span></span><br><ul><li><span data-ttu-id="ef1af-122">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1af-122">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="ef1af-123">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1af-123">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef1af-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef1af-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="ef1af-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1af-125">Request headers</span></span>

| <span data-ttu-id="ef1af-126">Nome</span><span class="sxs-lookup"><span data-stu-id="ef1af-126">Name</span></span>          | <span data-ttu-id="ef1af-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef1af-127">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ef1af-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef1af-128">Authorization</span></span> | <span data-ttu-id="ef1af-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef1af-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef1af-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef1af-131">Content-Type</span></span>  | <span data-ttu-id="ef1af-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef1af-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef1af-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1af-134">Request body</span></span>

<span data-ttu-id="ef1af-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef1af-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ef1af-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ef1af-136">Parameter</span></span>    | <span data-ttu-id="ef1af-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef1af-137">Type</span></span>        | <span data-ttu-id="ef1af-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef1af-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ef1af-139">ids</span><span class="sxs-lookup"><span data-stu-id="ef1af-139">ids</span></span>|<span data-ttu-id="ef1af-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef1af-140">String collection</span></span>| <span data-ttu-id="ef1af-141">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório ou IDs de roleTemplate das funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="ef1af-141">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="ef1af-142">Você pode especificar até 20 objetos.</span><span class="sxs-lookup"><span data-stu-id="ef1af-142">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="ef1af-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef1af-143">Response</span></span>

<span data-ttu-id="ef1af-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef1af-144">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef1af-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ef1af-145">Examples</span></span>

<span data-ttu-id="ef1af-146">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ef1af-146">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ef1af-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1af-147">Request</span></span>

<span data-ttu-id="ef1af-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef1af-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef1af-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef1af-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ef1af-150">C#</span><span class="sxs-lookup"><span data-stu-id="ef1af-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef1af-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef1af-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef1af-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef1af-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef1af-153">Java</span><span class="sxs-lookup"><span data-stu-id="ef1af-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ef1af-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef1af-154">Response</span></span>

<span data-ttu-id="ef1af-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ef1af-155">The following is an example of the response.</span></span> 

> <span data-ttu-id="ef1af-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef1af-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

