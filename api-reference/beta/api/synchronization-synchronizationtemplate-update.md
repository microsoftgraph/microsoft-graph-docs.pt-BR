---
title: Atualizar synchronizationtemplate
description: Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4327da9f4eb54c0e740370338806dc4078f2672c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452873"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="804d3-103">Atualizar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="804d3-103">Update synchronizationTemplate</span></span>

<span data-ttu-id="804d3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="804d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="804d3-105">Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="804d3-105">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="804d3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="804d3-106">Permissions</span></span>
<span data-ttu-id="804d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="804d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="804d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="804d3-109">Permission type</span></span>                        | <span data-ttu-id="804d3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="804d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="804d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="804d3-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="804d3-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="804d3-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="804d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="804d3-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="804d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804d3-114">Not supported.</span></span>|
|<span data-ttu-id="804d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="804d3-115">Application</span></span>                            |<span data-ttu-id="804d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804d3-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="804d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="804d3-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="804d3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="804d3-118">Request headers</span></span>

| <span data-ttu-id="804d3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="804d3-119">Name</span></span>           | <span data-ttu-id="804d3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="804d3-120">Type</span></span>    | <span data-ttu-id="804d3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="804d3-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="804d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="804d3-122">Authorization</span></span>  | <span data-ttu-id="804d3-123">string</span><span class="sxs-lookup"><span data-stu-id="804d3-123">string</span></span>  | <span data-ttu-id="804d3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="804d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="804d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="804d3-126">Request body</span></span>

<span data-ttu-id="804d3-127">No corpo da solicitação, forneça o objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="804d3-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="804d3-128">Certifique-se de que todas as propriedades sejam fornecidas.</span><span class="sxs-lookup"><span data-stu-id="804d3-128">Make sure all properties are provided.</span></span> <span data-ttu-id="804d3-129">As propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="804d3-129">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="804d3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="804d3-130">Response</span></span>

<span data-ttu-id="804d3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="804d3-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="804d3-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="804d3-133">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="804d3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="804d3-134">Request</span></span>
<span data-ttu-id="804d3-135">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="804d3-135">The following is an example of a request.</span></span> 

><span data-ttu-id="804d3-136">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="804d3-136">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="804d3-137">Incluir todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="804d3-137">Include all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="804d3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="804d3-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="804d3-139">C#</span><span class="sxs-lookup"><span data-stu-id="804d3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="804d3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="804d3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="804d3-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="804d3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="804d3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="804d3-142">Response</span></span>
<span data-ttu-id="804d3-143">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="804d3-143">The following is an example of a response.</span></span>
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
