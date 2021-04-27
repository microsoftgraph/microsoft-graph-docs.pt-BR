---
title: 'servicePrincipal: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Recupere da lista os grupos que o diretor de serviço tiver uma filiação direta ou transitória.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 6f530bf1f5bdb4a7bbb8353aa09471ed708b050b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051974"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="4b0bd-104">servicePrincipal: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="4b0bd-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="4b0bd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b0bd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b0bd-106">Verifique se há associação na lista de grupos especificada.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="4b0bd-107">Retorna da lista os grupos dos quais o [servicePrincipal](../resources/serviceprincipal.md) tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b0bd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b0bd-108">Permissions</span></span>
<span data-ttu-id="4b0bd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b0bd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b0bd-111">Permission type</span></span>      | <span data-ttu-id="4b0bd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b0bd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b0bd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b0bd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4b0bd-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b0bd-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4b0bd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b0bd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b0bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-116">Not supported.</span></span>    |
|<span data-ttu-id="4b0bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b0bd-117">Application</span></span> | <span data-ttu-id="4b0bd-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b0bd-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b0bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0bd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="4b0bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0bd-120">Request headers</span></span>
| <span data-ttu-id="4b0bd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4b0bd-121">Name</span></span>       | <span data-ttu-id="4b0bd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b0bd-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4b0bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b0bd-123">Authorization</span></span> | <span data-ttu-id="4b0bd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b0bd-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="4b0bd-126">Content-type</span></span> | <span data-ttu-id="4b0bd-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b0bd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0bd-129">Request body</span></span>
<span data-ttu-id="4b0bd-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b0bd-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4b0bd-131">Parameter</span></span>    | <span data-ttu-id="4b0bd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b0bd-132">Type</span></span>   |<span data-ttu-id="4b0bd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b0bd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b0bd-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="4b0bd-134">groupIds</span></span>|<span data-ttu-id="4b0bd-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b0bd-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="4b0bd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b0bd-136">Response</span></span>

<span data-ttu-id="4b0bd-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b0bd-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4b0bd-138">Examples</span></span>
<span data-ttu-id="4b0bd-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="4b0bd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0bd-140">Request</span></span>
<span data-ttu-id="4b0bd-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b0bd-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0bd-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="4b0bd-143">C#</span><span class="sxs-lookup"><span data-stu-id="4b0bd-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b0bd-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b0bd-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b0bd-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b0bd-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b0bd-146">Java</span><span class="sxs-lookup"><span data-stu-id="4b0bd-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4b0bd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b0bd-147">Response</span></span>
<span data-ttu-id="4b0bd-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-148">Here is an example of the response.</span></span> 
><span data-ttu-id="4b0bd-149">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b0bd-149">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



