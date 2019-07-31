---
title: Listar anexos
description: Obter uma lista de objetos Attachment anexados a uma tarefa do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 38da8bcbd0601bbca201b157db3d49d7016e2de3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988717"
---
# <a name="list-attachments"></a><span data-ttu-id="ab827-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="ab827-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab827-104">Obter uma lista de objetos [Attachment](../resources/attachment.md) anexados a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="ab827-104">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab827-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab827-105">Permissions</span></span>

<span data-ttu-id="ab827-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab827-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab827-108">Permission type</span></span>      | <span data-ttu-id="ab827-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab827-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab827-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab827-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab827-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ab827-111">Tasks.Read</span></span>    |
|<span data-ttu-id="ab827-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab827-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab827-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ab827-113">Tasks.Read</span></span>    |
|<span data-ttu-id="ab827-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab827-114">Application</span></span> | <span data-ttu-id="ab827-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab827-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab827-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab827-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab827-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab827-117">Optional query parameters</span></span>

<span data-ttu-id="ab827-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab827-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab827-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab827-119">Request headers</span></span>

| <span data-ttu-id="ab827-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ab827-120">Name</span></span>      |<span data-ttu-id="ab827-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab827-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab827-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab827-122">Authorization</span></span>  | <span data-ttu-id="ab827-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab827-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab827-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab827-125">Request body</span></span>

<span data-ttu-id="ab827-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab827-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab827-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab827-127">Response</span></span>

<span data-ttu-id="ab827-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab827-128">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab827-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab827-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab827-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab827-130">Request</span></span>

<span data-ttu-id="ab827-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab827-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ab827-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab827-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ab827-133">C#</span><span class="sxs-lookup"><span data-stu-id="ab827-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab827-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab827-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ab827-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ab827-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ab827-136">Java</span><span class="sxs-lookup"><span data-stu-id="ab827-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlook-task-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab827-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab827-137">Response</span></span>

<span data-ttu-id="ab827-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab827-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
