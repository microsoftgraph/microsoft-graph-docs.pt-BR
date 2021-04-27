---
title: Listar anexos
description: Obter uma lista de objetos anexos anexados a uma Outlook tarefa.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 87b7a341be4e280a8b211bf03e814006d8240755
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055474"
---
# <a name="list-attachments-deprecated"></a><span data-ttu-id="a7ff9-103">Anexos de lista (preterido)</span><span class="sxs-lookup"><span data-stu-id="a7ff9-103">List attachments (deprecated)</span></span>

<span data-ttu-id="a7ff9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7ff9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="a7ff9-105">Obter uma lista de [objetos anexos](../resources/attachment.md) anexados a uma Outlook tarefa.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-105">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7ff9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7ff9-106">Permissions</span></span>

<span data-ttu-id="a7ff9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7ff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7ff9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7ff9-109">Permission type</span></span>      | <span data-ttu-id="a7ff9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7ff9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7ff9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7ff9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7ff9-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a7ff9-112">Tasks.Read</span></span>    |
|<span data-ttu-id="a7ff9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7ff9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7ff9-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a7ff9-114">Tasks.Read</span></span>    |
|<span data-ttu-id="a7ff9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7ff9-115">Application</span></span> | <span data-ttu-id="a7ff9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7ff9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7ff9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7ff9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7ff9-118">Optional query parameters</span></span>

<span data-ttu-id="a7ff9-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7ff9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ff9-120">Request headers</span></span>

| <span data-ttu-id="a7ff9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a7ff9-121">Name</span></span>      |<span data-ttu-id="a7ff9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7ff9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a7ff9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7ff9-123">Authorization</span></span>  | <span data-ttu-id="a7ff9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7ff9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ff9-126">Request body</span></span>

<span data-ttu-id="a7ff9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7ff9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ff9-128">Response</span></span>

<span data-ttu-id="a7ff9-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [anexos](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-129">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7ff9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7ff9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7ff9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ff9-131">Request</span></span>

<span data-ttu-id="a7ff9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7ff9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7ff9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="a7ff9-134">C#</span><span class="sxs-lookup"><span data-stu-id="a7ff9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7ff9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7ff9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7ff9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7ff9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7ff9-137">Java</span><span class="sxs-lookup"><span data-stu-id="a7ff9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlook-task-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a7ff9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ff9-138">Response</span></span>

<span data-ttu-id="a7ff9-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-139">Here is an example of the response.</span></span> <span data-ttu-id="a7ff9-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a7ff9-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
