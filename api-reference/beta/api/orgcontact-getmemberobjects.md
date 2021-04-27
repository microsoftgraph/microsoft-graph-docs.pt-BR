---
title: 'orgContact: getMemberObjects'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1187661bff6257fcb7c009a38b5cbc8e2388ea04
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055544"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="a4437-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a4437-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="a4437-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4437-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="a4437-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4437-106">Permissions</span></span>
<span data-ttu-id="a4437-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4437-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4437-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4437-109">Permission type</span></span>      | <span data-ttu-id="a4437-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4437-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4437-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4437-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4437-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4437-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4437-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4437-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4437-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4437-114">Not supported.</span></span>    |
|<span data-ttu-id="a4437-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4437-115">Application</span></span> | <span data-ttu-id="a4437-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4437-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4437-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4437-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="a4437-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4437-118">Request headers</span></span>
| <span data-ttu-id="a4437-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a4437-119">Name</span></span>       | <span data-ttu-id="a4437-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4437-120">Type</span></span> | <span data-ttu-id="a4437-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4437-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a4437-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4437-122">Authorization</span></span>  | <span data-ttu-id="a4437-123">string</span><span class="sxs-lookup"><span data-stu-id="a4437-123">string</span></span>  | <span data-ttu-id="a4437-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4437-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4437-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4437-126">Request body</span></span>
<span data-ttu-id="a4437-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4437-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4437-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4437-128">Parameter</span></span>    | <span data-ttu-id="a4437-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4437-129">Type</span></span>   |<span data-ttu-id="a4437-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4437-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4437-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a4437-131">securityEnabledOnly</span></span>|<span data-ttu-id="a4437-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4437-132">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="a4437-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4437-133">Response</span></span>

<span data-ttu-id="a4437-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4437-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4437-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4437-135">Example</span></span>
<span data-ttu-id="a4437-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a4437-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4437-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4437-137">Request</span></span>
<span data-ttu-id="a4437-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4437-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4437-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4437-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="a4437-140">C#</span><span class="sxs-lookup"><span data-stu-id="a4437-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4437-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4437-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4437-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4437-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4437-143">Java</span><span class="sxs-lookup"><span data-stu-id="a4437-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4437-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4437-144">Response</span></span>
<span data-ttu-id="a4437-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4437-145">Here is an example of the response.</span></span> <span data-ttu-id="a4437-146">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4437-146">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


