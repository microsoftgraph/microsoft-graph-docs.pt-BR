---
title: Listar categorias do Outlook
description: Obtém todas as categorias que foram definidas para o usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5da75dca3e5bee628284a8f09ae6221b6a3a67f5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349720"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="848de-103">Listar categorias do Outlook</span><span class="sxs-lookup"><span data-stu-id="848de-103">List Outlook categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="848de-104">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="848de-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="848de-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="848de-105">Permissions</span></span>
<span data-ttu-id="848de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="848de-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="848de-108">Permission type</span></span>      | <span data-ttu-id="848de-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="848de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="848de-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="848de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="848de-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="848de-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="848de-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="848de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="848de-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="848de-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="848de-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="848de-114">Application</span></span> | <span data-ttu-id="848de-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="848de-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="848de-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="848de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="848de-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="848de-117">Optional query parameters</span></span>
<span data-ttu-id="848de-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="848de-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="848de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="848de-119">Request headers</span></span>
| <span data-ttu-id="848de-120">Nome</span><span class="sxs-lookup"><span data-stu-id="848de-120">Name</span></span>      |<span data-ttu-id="848de-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="848de-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="848de-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="848de-122">Authorization</span></span>  | <span data-ttu-id="848de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="848de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="848de-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="848de-125">Request body</span></span>
<span data-ttu-id="848de-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="848de-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="848de-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="848de-127">Response</span></span>

<span data-ttu-id="848de-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="848de-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="848de-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="848de-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="848de-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="848de-130">Request</span></span>
<span data-ttu-id="848de-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="848de-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="848de-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="848de-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="848de-133">C#</span><span class="sxs-lookup"><span data-stu-id="848de-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mastercategories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="848de-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="848de-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mastercategories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="848de-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="848de-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mastercategories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="848de-136">Java</span><span class="sxs-lookup"><span data-stu-id="848de-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mastercategories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="848de-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="848de-137">Response</span></span>
<span data-ttu-id="848de-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="848de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
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
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
