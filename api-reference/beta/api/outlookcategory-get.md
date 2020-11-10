---
title: Obter categoria do Outlook
description: Obtenha as propriedades e as relações do objeto outlookCategory especificado.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 43f1ab353a1fbce12b3b0bf674cce43dd0eff039
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972836"
---
# <a name="get-outlook-category"></a><span data-ttu-id="499ec-103">Obter categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="499ec-103">Get Outlook category</span></span>

<span data-ttu-id="499ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="499ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="499ec-105">Obtenha as propriedades e as relações do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="499ec-105">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="499ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="499ec-106">Permissions</span></span>
<span data-ttu-id="499ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="499ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="499ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="499ec-109">Permission type</span></span>      | <span data-ttu-id="499ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="499ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="499ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="499ec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="499ec-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="499ec-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="499ec-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="499ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="499ec-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="499ec-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="499ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="499ec-115">Application</span></span> | <span data-ttu-id="499ec-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="499ec-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="499ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="499ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="499ec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="499ec-118">Optional query parameters</span></span>
<span data-ttu-id="499ec-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="499ec-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="499ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="499ec-120">Request headers</span></span>
| <span data-ttu-id="499ec-121">Nome</span><span class="sxs-lookup"><span data-stu-id="499ec-121">Name</span></span>      |<span data-ttu-id="499ec-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="499ec-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="499ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="499ec-123">Authorization</span></span>  | <span data-ttu-id="499ec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="499ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="499ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="499ec-126">Request body</span></span>
<span data-ttu-id="499ec-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="499ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="499ec-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="499ec-128">Response</span></span>

<span data-ttu-id="499ec-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="499ec-129">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="499ec-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="499ec-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="499ec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="499ec-131">Request</span></span>
<span data-ttu-id="499ec-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="499ec-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="499ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="499ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
# <a name="c"></a>[<span data-ttu-id="499ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="499ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="499ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="499ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="499ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="499ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="499ec-137">Java</span><span class="sxs-lookup"><span data-stu-id="499ec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="499ec-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="499ec-138">Response</span></span>
<span data-ttu-id="499ec-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="499ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
