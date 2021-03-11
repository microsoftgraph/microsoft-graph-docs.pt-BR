---
title: Atualizar synchronizationTemplate
description: Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 133f503ee6361619581cea058fbf3a47a8c7de01
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722010"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="38a1c-103">Atualizar synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="38a1c-103">Update synchronizationTemplate</span></span>

<span data-ttu-id="38a1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a1c-105">Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="38a1c-105">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="38a1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38a1c-106">Permissions</span></span>
<span data-ttu-id="38a1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38a1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38a1c-109">Permission type</span></span>                        | <span data-ttu-id="38a1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38a1c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="38a1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38a1c-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="38a1c-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a1c-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="38a1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38a1c-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="38a1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38a1c-114">Not supported.</span></span>|
|<span data-ttu-id="38a1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38a1c-115">Application</span></span>                            |<span data-ttu-id="38a1c-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a1c-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="38a1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38a1c-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH applications/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="38a1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38a1c-118">Request headers</span></span>

| <span data-ttu-id="38a1c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="38a1c-119">Name</span></span>           | <span data-ttu-id="38a1c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="38a1c-120">Type</span></span>    | <span data-ttu-id="38a1c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a1c-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="38a1c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38a1c-122">Authorization</span></span>  | <span data-ttu-id="38a1c-123">string</span><span class="sxs-lookup"><span data-stu-id="38a1c-123">string</span></span>  | <span data-ttu-id="38a1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38a1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38a1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38a1c-126">Request body</span></span>

<span data-ttu-id="38a1c-127">No corpo da solicitação, fornece o [objeto synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="38a1c-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="38a1c-128">Certifique-se de que todas as propriedades sejam fornecidas.</span><span class="sxs-lookup"><span data-stu-id="38a1c-128">Make sure all properties are provided.</span></span> <span data-ttu-id="38a1c-129">Propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="38a1c-129">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="38a1c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="38a1c-130">Response</span></span>

<span data-ttu-id="38a1c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38a1c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="38a1c-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="38a1c-133">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="38a1c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38a1c-134">Request</span></span>
<span data-ttu-id="38a1c-135">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="38a1c-135">The following is an example of a request.</span></span> 

><span data-ttu-id="38a1c-136">**Observação:** O objeto request mostrado aqui é reduzido para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="38a1c-136">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="38a1c-137">Inclua todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38a1c-137">Include all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="38a1c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="38a1c-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="38a1c-139">C#</span><span class="sxs-lookup"><span data-stu-id="38a1c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38a1c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38a1c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38a1c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38a1c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38a1c-142">Java</span><span class="sxs-lookup"><span data-stu-id="38a1c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="38a1c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="38a1c-143">Response</span></span>
<span data-ttu-id="38a1c-144">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="38a1c-144">The following is an example of a response.</span></span>
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


