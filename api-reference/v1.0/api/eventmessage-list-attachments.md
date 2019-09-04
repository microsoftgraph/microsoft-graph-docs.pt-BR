---
title: Listar anexos
description: Recupera uma lista de objetos de anexo.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ad35162d356a7961af5961c680005be04d191425
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726806"
---
# <a name="list-attachments"></a><span data-ttu-id="5bd30-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="5bd30-103">List attachments</span></span>

<span data-ttu-id="5bd30-104">Recupera uma lista de objetos de anexo.</span><span class="sxs-lookup"><span data-stu-id="5bd30-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5bd30-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bd30-105">Permissions</span></span>
<span data-ttu-id="5bd30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bd30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bd30-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bd30-108">Permission type</span></span>      | <span data-ttu-id="5bd30-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bd30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bd30-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bd30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5bd30-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5bd30-111">Mail.Read</span></span>    |
|<span data-ttu-id="5bd30-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bd30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bd30-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5bd30-113">Mail.Read</span></span>    |
|<span data-ttu-id="5bd30-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bd30-114">Application</span></span> | <span data-ttu-id="5bd30-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5bd30-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bd30-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bd30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5bd30-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5bd30-117">Optional query parameters</span></span>
<span data-ttu-id="5bd30-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5bd30-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bd30-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bd30-119">Request headers</span></span>
| <span data-ttu-id="5bd30-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5bd30-120">Name</span></span>       | <span data-ttu-id="5bd30-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bd30-121">Type</span></span> | <span data-ttu-id="5bd30-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bd30-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5bd30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bd30-123">Authorization</span></span>  | <span data-ttu-id="5bd30-124">string</span><span class="sxs-lookup"><span data-stu-id="5bd30-124">string</span></span>  | <span data-ttu-id="5bd30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bd30-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bd30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bd30-127">Request body</span></span>
<span data-ttu-id="5bd30-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5bd30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bd30-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bd30-129">Response</span></span>

<span data-ttu-id="5bd30-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bd30-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5bd30-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bd30-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bd30-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bd30-132">Request</span></span>
<span data-ttu-id="5bd30-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bd30-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5bd30-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bd30-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5bd30-135">C#</span><span class="sxs-lookup"><span data-stu-id="5bd30-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bd30-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bd30-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5bd30-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5bd30-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5bd30-138">Java</span><span class="sxs-lookup"><span data-stu-id="5bd30-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/eventmessage-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5bd30-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bd30-139">Response</span></span>
<span data-ttu-id="5bd30-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bd30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "eventmessage_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
