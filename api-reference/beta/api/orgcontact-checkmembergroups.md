---
title: 'orgContact: checkMemberGroups'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3abbd7162759fa53103c1a49bb737870412dcfe1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342478"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="3f4f2-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3f4f2-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="3f4f2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f4f2-105">Permissions</span></span>
<span data-ttu-id="3f4f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f4f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f4f2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f4f2-108">Permission type</span></span>      | <span data-ttu-id="3f4f2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f4f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f4f2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f4f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f4f2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f4f2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f4f2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f4f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f4f2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-113">Not supported.</span></span>    |
|<span data-ttu-id="3f4f2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f4f2-114">Application</span></span> | <span data-ttu-id="3f4f2-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f4f2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f4f2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f4f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="3f4f2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f4f2-117">Request headers</span></span>
| <span data-ttu-id="3f4f2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3f4f2-118">Name</span></span>       | <span data-ttu-id="3f4f2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f4f2-119">Type</span></span> | <span data-ttu-id="3f4f2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f4f2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3f4f2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f4f2-121">Authorization</span></span>  | <span data-ttu-id="3f4f2-122">string</span><span class="sxs-lookup"><span data-stu-id="3f4f2-122">string</span></span>  | <span data-ttu-id="3f4f2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f4f2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f4f2-125">Request body</span></span>
<span data-ttu-id="3f4f2-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3f4f2-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3f4f2-127">Parameter</span></span>    | <span data-ttu-id="3f4f2-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f4f2-128">Type</span></span>   |<span data-ttu-id="3f4f2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f4f2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f4f2-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="3f4f2-130">groupIds</span></span>|<span data-ttu-id="3f4f2-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f4f2-131">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="3f4f2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f4f2-132">Response</span></span>

<span data-ttu-id="3f4f2-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f4f2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f4f2-134">Example</span></span>
<span data-ttu-id="3f4f2-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3f4f2-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f4f2-136">Request</span></span>
<span data-ttu-id="3f4f2-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f4f2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f4f2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f4f2-139">C#</span><span class="sxs-lookup"><span data-stu-id="3f4f2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f4f2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f4f2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f4f2-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3f4f2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3f4f2-142">Java</span><span class="sxs-lookup"><span data-stu-id="3f4f2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f4f2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f4f2-143">Response</span></span>
<span data-ttu-id="3f4f2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
