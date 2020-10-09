---
title: Listar anexos
description: Recupera uma lista de objetos de anexo.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 54e82e8946b33bf900fd808d7b135168250b885a
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401320"
---
# <a name="list-attachments"></a><span data-ttu-id="d7871-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="d7871-103">List attachments</span></span>

<span data-ttu-id="d7871-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7871-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7871-105">Recupera uma lista de objetos de anexo.</span><span class="sxs-lookup"><span data-stu-id="d7871-105">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7871-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7871-106">Permissions</span></span>
<span data-ttu-id="d7871-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7871-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7871-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7871-109">Permission type</span></span>      | <span data-ttu-id="d7871-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7871-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7871-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7871-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d7871-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d7871-112">Mail.Read</span></span>    |
|<span data-ttu-id="d7871-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7871-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7871-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d7871-114">Mail.Read</span></span>    |
|<span data-ttu-id="d7871-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7871-115">Application</span></span> | <span data-ttu-id="d7871-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d7871-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7871-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7871-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7871-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d7871-118">Optional query parameters</span></span>
<span data-ttu-id="d7871-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d7871-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7871-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7871-120">Request headers</span></span>
| <span data-ttu-id="d7871-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d7871-121">Name</span></span>       | <span data-ttu-id="d7871-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7871-122">Type</span></span> | <span data-ttu-id="d7871-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7871-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7871-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7871-124">Authorization</span></span>  | <span data-ttu-id="d7871-125">string</span><span class="sxs-lookup"><span data-stu-id="d7871-125">string</span></span>  | <span data-ttu-id="d7871-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7871-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7871-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7871-128">Request body</span></span>
<span data-ttu-id="d7871-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7871-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7871-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7871-130">Response</span></span>

<span data-ttu-id="d7871-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7871-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7871-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7871-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7871-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7871-133">Request</span></span>
<span data-ttu-id="d7871-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7871-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7871-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7871-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="d7871-136">C#</span><span class="sxs-lookup"><span data-stu-id="d7871-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7871-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7871-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7871-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7871-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7871-139">Java</span><span class="sxs-lookup"><span data-stu-id="d7871-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/eventmessage-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7871-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7871-140">Response</span></span>
<span data-ttu-id="d7871-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7871-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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