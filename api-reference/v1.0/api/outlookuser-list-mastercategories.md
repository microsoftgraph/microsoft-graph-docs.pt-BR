---
title: Listar categorias do Outlook
description: Obtém todas as categorias que foram definidas para o usuário.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d14d477d3f2a7be94a676aafd17eee6ebf362925
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089025"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="b3225-103">Listar categorias do Outlook</span><span class="sxs-lookup"><span data-stu-id="b3225-103">List Outlook categories</span></span>

<span data-ttu-id="b3225-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3225-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b3225-105">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b3225-105">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3225-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3225-106">Permissions</span></span>
<span data-ttu-id="b3225-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3225-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3225-109">Permission type</span></span>      | <span data-ttu-id="b3225-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3225-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3225-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3225-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3225-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b3225-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b3225-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3225-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3225-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b3225-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b3225-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3225-115">Application</span></span> | <span data-ttu-id="b3225-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b3225-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3225-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3225-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3225-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3225-118">Optional query parameters</span></span>
<span data-ttu-id="b3225-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3225-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3225-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3225-120">Request headers</span></span>
| <span data-ttu-id="b3225-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b3225-121">Name</span></span>      |<span data-ttu-id="b3225-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3225-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3225-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3225-123">Authorization</span></span>  | <span data-ttu-id="b3225-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3225-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3225-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3225-126">Request body</span></span>
<span data-ttu-id="b3225-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3225-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3225-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3225-128">Response</span></span>

<span data-ttu-id="b3225-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3225-129">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3225-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3225-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3225-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3225-131">Request</span></span>
<span data-ttu-id="b3225-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3225-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3225-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3225-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories
```
# <a name="c"></a>[<span data-ttu-id="b3225-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3225-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mastercategories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3225-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3225-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mastercategories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3225-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3225-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mastercategories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3225-137">Java</span><span class="sxs-lookup"><span data-stu-id="b3225-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mastercategories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3225-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3225-138">Response</span></span>
<span data-ttu-id="b3225-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3225-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

