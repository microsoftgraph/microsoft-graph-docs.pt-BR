---
title: 'servicePrincipal: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos dos quais a entidade de serviço tem uma associação direta ou transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: bca8a52ea2d10ba4dd32e871ab0dbadcf454bf00
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025393"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="89e7d-104">servicePrincipal: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="89e7d-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="89e7d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e7d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89e7d-106">Verifique se há associação na lista de grupos especificada.</span><span class="sxs-lookup"><span data-stu-id="89e7d-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="89e7d-107">Retorna da lista os grupos dos quais o [servicePrincipal](../resources/serviceprincipal.md) tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="89e7d-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="89e7d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="89e7d-108">Permissions</span></span>
<span data-ttu-id="89e7d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e7d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e7d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89e7d-111">Permission type</span></span>      | <span data-ttu-id="89e7d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89e7d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89e7d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89e7d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="89e7d-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89e7d-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89e7d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89e7d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89e7d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89e7d-116">Not supported.</span></span>    |
|<span data-ttu-id="89e7d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89e7d-117">Application</span></span> | <span data-ttu-id="89e7d-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="89e7d-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89e7d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="89e7d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7d-120">Request headers</span></span>
| <span data-ttu-id="89e7d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="89e7d-121">Name</span></span>       | <span data-ttu-id="89e7d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="89e7d-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="89e7d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89e7d-123">Authorization</span></span> | <span data-ttu-id="89e7d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89e7d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89e7d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89e7d-126">Content-Type</span></span> | <span data-ttu-id="89e7d-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89e7d-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89e7d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7d-129">Request body</span></span>
<span data-ttu-id="89e7d-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e7d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="89e7d-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="89e7d-131">Parameter</span></span>    | <span data-ttu-id="89e7d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="89e7d-132">Type</span></span>   |<span data-ttu-id="89e7d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="89e7d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89e7d-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="89e7d-134">groupIds</span></span>|<span data-ttu-id="89e7d-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="89e7d-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="89e7d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7d-136">Response</span></span>

<span data-ttu-id="89e7d-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89e7d-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89e7d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89e7d-138">Examples</span></span>
<span data-ttu-id="89e7d-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="89e7d-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="89e7d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7d-140">Request</span></span>
<span data-ttu-id="89e7d-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e7d-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="89e7d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="89e7d-143">C#</span><span class="sxs-lookup"><span data-stu-id="89e7d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89e7d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89e7d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89e7d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89e7d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89e7d-146">Java</span><span class="sxs-lookup"><span data-stu-id="89e7d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="89e7d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7d-147">Response</span></span>
<span data-ttu-id="89e7d-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89e7d-148">Here is an example of the response.</span></span> 
><span data-ttu-id="89e7d-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89e7d-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

