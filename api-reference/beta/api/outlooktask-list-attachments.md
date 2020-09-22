---
title: Listar anexos
description: Obter uma lista de objetos Attachment anexados a uma tarefa do Outlook.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 60626ade5e83366520bc3c34dd7002cae36e1180
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017416"
---
# <a name="list-attachments-deprecated"></a><span data-ttu-id="24672-103">Listar anexos (preterido)</span><span class="sxs-lookup"><span data-stu-id="24672-103">List attachments (deprecated)</span></span>

<span data-ttu-id="24672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24672-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="24672-105">Obter uma lista de objetos [Attachment](../resources/attachment.md) anexados a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="24672-105">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="24672-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24672-106">Permissions</span></span>

<span data-ttu-id="24672-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24672-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24672-109">Permission type</span></span>      | <span data-ttu-id="24672-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24672-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24672-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24672-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24672-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="24672-112">Tasks.Read</span></span>    |
|<span data-ttu-id="24672-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24672-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24672-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="24672-114">Tasks.Read</span></span>    |
|<span data-ttu-id="24672-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24672-115">Application</span></span> | <span data-ttu-id="24672-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24672-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24672-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24672-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24672-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24672-118">Optional query parameters</span></span>

<span data-ttu-id="24672-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24672-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24672-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24672-120">Request headers</span></span>

| <span data-ttu-id="24672-121">Nome</span><span class="sxs-lookup"><span data-stu-id="24672-121">Name</span></span>      |<span data-ttu-id="24672-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="24672-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24672-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24672-123">Authorization</span></span>  | <span data-ttu-id="24672-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24672-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24672-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24672-126">Request body</span></span>

<span data-ttu-id="24672-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24672-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24672-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="24672-128">Response</span></span>

<span data-ttu-id="24672-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24672-129">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24672-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24672-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="24672-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24672-131">Request</span></span>

<span data-ttu-id="24672-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24672-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="24672-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="24672-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="24672-134">C#</span><span class="sxs-lookup"><span data-stu-id="24672-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24672-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24672-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24672-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24672-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24672-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="24672-137">Response</span></span>

<span data-ttu-id="24672-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24672-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


