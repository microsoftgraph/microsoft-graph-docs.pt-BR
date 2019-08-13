---
title: Atualizar synchronizationtemplate
description: Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 05c91fe33116c47c2cbe145a106ac467db76ae8a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363386"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="c51c1-103">Atualizar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="c51c1-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c51c1-104">Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c51c1-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c51c1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c51c1-105">Permissions</span></span>
<span data-ttu-id="c51c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c51c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51c1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c51c1-108">Permission type</span></span>                        | <span data-ttu-id="c51c1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c51c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c51c1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c51c1-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="c51c1-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c51c1-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c51c1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c51c1-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c51c1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c51c1-113">Not supported.</span></span>|
|<span data-ttu-id="c51c1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c51c1-114">Application</span></span>                            |<span data-ttu-id="c51c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c51c1-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="c51c1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c51c1-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="c51c1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c51c1-117">Request headers</span></span>

| <span data-ttu-id="c51c1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c51c1-118">Name</span></span>           | <span data-ttu-id="c51c1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c51c1-119">Type</span></span>    | <span data-ttu-id="c51c1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c51c1-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c51c1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c51c1-121">Authorization</span></span>  | <span data-ttu-id="c51c1-122">string</span><span class="sxs-lookup"><span data-stu-id="c51c1-122">string</span></span>  | <span data-ttu-id="c51c1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c51c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c51c1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c51c1-125">Request body</span></span>

<span data-ttu-id="c51c1-126">No corpo da solicitação, forneça o [](../resources/synchronization-synchronizationtemplate.md) objeto synchronizationtemplate para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="c51c1-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="c51c1-127">Certifique-se de que todas as propriedades sejam fornecidas.</span><span class="sxs-lookup"><span data-stu-id="c51c1-127">Make sure all properties are provided.</span></span> <span data-ttu-id="c51c1-128">As propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="c51c1-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="c51c1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c51c1-129">Response</span></span>

<span data-ttu-id="c51c1-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c51c1-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="c51c1-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c51c1-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="c51c1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c51c1-133">Request</span></span>
<span data-ttu-id="c51c1-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c51c1-134">The following is an example of a request.</span></span> 

><span data-ttu-id="c51c1-135">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c51c1-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="c51c1-136">Incluir todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c51c1-136">Include all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c51c1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c51c1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c51c1-138">C#</span><span class="sxs-lookup"><span data-stu-id="c51c1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c51c1-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c51c1-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c51c1-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c51c1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c51c1-141">Java</span><span class="sxs-lookup"><span data-stu-id="c51c1-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c51c1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c51c1-142">Response</span></span>
<span data-ttu-id="c51c1-143">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c51c1-143">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
