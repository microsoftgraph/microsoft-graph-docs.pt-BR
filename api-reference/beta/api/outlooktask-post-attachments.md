---
title: Criar anexo
description: Use esta API para adicionar um anexo a um outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d48b04d6c5882cc5b90eaec2138f1070f8b4db7b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877671"
---
# <a name="create-attachment"></a><span data-ttu-id="af7fd-103">Criar anexo</span><span class="sxs-lookup"><span data-stu-id="af7fd-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af7fd-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a um [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="af7fd-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af7fd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="af7fd-105">Permissions</span></span>

<span data-ttu-id="af7fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af7fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af7fd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af7fd-108">Permission type</span></span>      | <span data-ttu-id="af7fd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af7fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af7fd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af7fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af7fd-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af7fd-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="af7fd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af7fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af7fd-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af7fd-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="af7fd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af7fd-114">Application</span></span> | <span data-ttu-id="af7fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af7fd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af7fd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af7fd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="af7fd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af7fd-117">Request headers</span></span>

| <span data-ttu-id="af7fd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="af7fd-118">Name</span></span>       | <span data-ttu-id="af7fd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="af7fd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="af7fd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="af7fd-120">Authorization</span></span>  | <span data-ttu-id="af7fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af7fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af7fd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af7fd-123">Content-Type</span></span> | <span data-ttu-id="af7fd-124">Uma cadeia de caracteres que representa o tipo de dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="af7fd-124">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="af7fd-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af7fd-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af7fd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af7fd-126">Request body</span></span>

<span data-ttu-id="af7fd-127">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="af7fd-127">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="af7fd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="af7fd-128">Response</span></span>

<span data-ttu-id="af7fd-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af7fd-129">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af7fd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af7fd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="af7fd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af7fd-131">Request</span></span>

<span data-ttu-id="af7fd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af7fd-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="af7fd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="af7fd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_attachment_from_outlooktask"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af7fd-134">C#</span><span class="sxs-lookup"><span data-stu-id="af7fd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-attachment-from-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af7fd-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="af7fd-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-attachment-from-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="af7fd-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="af7fd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-attachment-from-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="af7fd-137">Java</span><span class="sxs-lookup"><span data-stu-id="af7fd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-attachment-from-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="af7fd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="af7fd-138">Response</span></span>

<span data-ttu-id="af7fd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af7fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
