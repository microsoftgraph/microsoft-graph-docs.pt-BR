---
title: 'orgContact: getMemberGroups'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f9aea52388a64355989ff78c222b00ff893e3473
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055551"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="6ea06-104">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="6ea06-104">orgContact: getMemberGroups</span></span>

<span data-ttu-id="6ea06-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ea06-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="6ea06-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ea06-106">Permissions</span></span>
<span data-ttu-id="6ea06-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ea06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ea06-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ea06-109">Permission type</span></span>      | <span data-ttu-id="6ea06-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ea06-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ea06-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ea06-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ea06-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ea06-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ea06-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ea06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ea06-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ea06-114">Not supported.</span></span>    |
|<span data-ttu-id="6ea06-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ea06-115">Application</span></span> | <span data-ttu-id="6ea06-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ea06-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ea06-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea06-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="6ea06-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea06-118">Request headers</span></span>
| <span data-ttu-id="6ea06-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6ea06-119">Name</span></span>       | <span data-ttu-id="6ea06-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ea06-120">Type</span></span> | <span data-ttu-id="6ea06-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea06-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ea06-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ea06-122">Authorization</span></span>  | <span data-ttu-id="6ea06-123">string</span><span class="sxs-lookup"><span data-stu-id="6ea06-123">string</span></span>  | <span data-ttu-id="6ea06-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ea06-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ea06-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea06-126">Request body</span></span>
<span data-ttu-id="6ea06-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ea06-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6ea06-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6ea06-128">Parameter</span></span>    | <span data-ttu-id="6ea06-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ea06-129">Type</span></span>   |<span data-ttu-id="6ea06-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea06-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ea06-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6ea06-131">securityEnabledOnly</span></span>|<span data-ttu-id="6ea06-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ea06-132">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="6ea06-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea06-133">Response</span></span>

<span data-ttu-id="6ea06-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ea06-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ea06-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ea06-135">Example</span></span>
<span data-ttu-id="6ea06-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6ea06-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6ea06-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea06-137">Request</span></span>
<span data-ttu-id="6ea06-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ea06-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ea06-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea06-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="6ea06-140">C#</span><span class="sxs-lookup"><span data-stu-id="6ea06-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ea06-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ea06-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ea06-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ea06-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ea06-143">Java</span><span class="sxs-lookup"><span data-stu-id="6ea06-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6ea06-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea06-144">Response</span></span>
<span data-ttu-id="6ea06-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ea06-145">Here is an example of the response.</span></span> <span data-ttu-id="6ea06-146">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6ea06-146">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


