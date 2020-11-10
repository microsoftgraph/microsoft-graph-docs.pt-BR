---
title: 'orgContact: getMemberGroups'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 83c17963db08bc0cc479ee94a4d4dc6859b0d86f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979030"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="b556a-104">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b556a-104">orgContact: getMemberGroups</span></span>

<span data-ttu-id="b556a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b556a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="b556a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b556a-106">Permissions</span></span>
<span data-ttu-id="b556a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b556a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b556a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b556a-109">Permission type</span></span>      | <span data-ttu-id="b556a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b556a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b556a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b556a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b556a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b556a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b556a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b556a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b556a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b556a-114">Not supported.</span></span>    |
|<span data-ttu-id="b556a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b556a-115">Application</span></span> | <span data-ttu-id="b556a-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b556a-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b556a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b556a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="b556a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b556a-118">Request headers</span></span>
| <span data-ttu-id="b556a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b556a-119">Name</span></span>       | <span data-ttu-id="b556a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b556a-120">Type</span></span> | <span data-ttu-id="b556a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b556a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b556a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b556a-122">Authorization</span></span>  | <span data-ttu-id="b556a-123">string</span><span class="sxs-lookup"><span data-stu-id="b556a-123">string</span></span>  | <span data-ttu-id="b556a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b556a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b556a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b556a-126">Request body</span></span>
<span data-ttu-id="b556a-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b556a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b556a-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b556a-128">Parameter</span></span>    | <span data-ttu-id="b556a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b556a-129">Type</span></span>   |<span data-ttu-id="b556a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b556a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b556a-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b556a-131">securityEnabledOnly</span></span>|<span data-ttu-id="b556a-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="b556a-132">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="b556a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b556a-133">Response</span></span>

<span data-ttu-id="b556a-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b556a-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b556a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b556a-135">Example</span></span>
<span data-ttu-id="b556a-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b556a-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b556a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b556a-137">Request</span></span>
<span data-ttu-id="b556a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b556a-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b556a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b556a-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b556a-140">C#</span><span class="sxs-lookup"><span data-stu-id="b556a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b556a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b556a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b556a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b556a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b556a-143">Java</span><span class="sxs-lookup"><span data-stu-id="b556a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b556a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b556a-144">Response</span></span>
<span data-ttu-id="b556a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b556a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


