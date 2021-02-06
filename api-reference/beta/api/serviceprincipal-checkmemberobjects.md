---
title: 'servicePrincipal: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de entidade de serviço especificado.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: a0bf3389563f99b69b7e27651f85163e7f820748
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135916"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="150ec-103">servicePrincipal: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="150ec-103">servicePrincipal: checkMemberObjects</span></span>

<span data-ttu-id="150ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="150ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="150ec-105">Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto [servicePrincipal](../resources/serviceprincipal.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="150ec-105">Check for membership in a list of groups, directory roles, or administrative units for the specified [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="150ec-106">Esse método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="150ec-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="150ec-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="150ec-107">Permissions</span></span>

<span data-ttu-id="150ec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="150ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="150ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="150ec-110">Permission type</span></span>                        | <span data-ttu-id="150ec-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="150ec-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="150ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="150ec-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="150ec-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="150ec-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="150ec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="150ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="150ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="150ec-115">Not supported.</span></span> |
| <span data-ttu-id="150ec-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="150ec-116">Application</span></span>                            | <span data-ttu-id="150ec-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="150ec-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="150ec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="150ec-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="150ec-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="150ec-119">Request headers</span></span>

| <span data-ttu-id="150ec-120">Nome</span><span class="sxs-lookup"><span data-stu-id="150ec-120">Name</span></span>          | <span data-ttu-id="150ec-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="150ec-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="150ec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="150ec-122">Authorization</span></span> | <span data-ttu-id="150ec-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="150ec-123">Bearer {token}</span></span> |
| <span data-ttu-id="150ec-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="150ec-124">Content-Type</span></span>  | <span data-ttu-id="150ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="150ec-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="150ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="150ec-126">Request body</span></span>

<span data-ttu-id="150ec-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="150ec-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="150ec-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="150ec-128">Parameter</span></span>    | <span data-ttu-id="150ec-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="150ec-129">Type</span></span>        | <span data-ttu-id="150ec-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="150ec-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="150ec-131">ids</span><span class="sxs-lookup"><span data-stu-id="150ec-131">ids</span></span>|<span data-ttu-id="150ec-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="150ec-132">String collection</span></span>|<span data-ttu-id="150ec-133">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs de roleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="150ec-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="150ec-134">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="150ec-134">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="150ec-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="150ec-135">Response</span></span>

<span data-ttu-id="150ec-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="150ec-136">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="150ec-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="150ec-137">Examples</span></span>

<span data-ttu-id="150ec-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="150ec-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="150ec-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="150ec-139">Request</span></span>

<span data-ttu-id="150ec-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="150ec-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="150ec-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="150ec-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="150ec-142">C#</span><span class="sxs-lookup"><span data-stu-id="150ec-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="150ec-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="150ec-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="150ec-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="150ec-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="150ec-145">Java</span><span class="sxs-lookup"><span data-stu-id="150ec-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="150ec-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="150ec-146">Response</span></span>

<span data-ttu-id="150ec-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="150ec-147">The following is an example of the response.</span></span> 

> <span data-ttu-id="150ec-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="150ec-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "servicePrincipal: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



