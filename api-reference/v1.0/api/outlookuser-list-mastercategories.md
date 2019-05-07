---
title: Listar categorias do Outlook
description: Obtém todas as categorias que foram definidas para o usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c485f14e293d6375d9739c819dc953137833609b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611861"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="975bf-103">Listar categorias do Outlook</span><span class="sxs-lookup"><span data-stu-id="975bf-103">List Outlook categories</span></span>


<span data-ttu-id="975bf-104">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="975bf-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="975bf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="975bf-105">Permissions</span></span>
<span data-ttu-id="975bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="975bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="975bf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="975bf-108">Permission type</span></span>      | <span data-ttu-id="975bf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="975bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="975bf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="975bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="975bf-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="975bf-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="975bf-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="975bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="975bf-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="975bf-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="975bf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="975bf-114">Application</span></span> | <span data-ttu-id="975bf-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="975bf-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="975bf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="975bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="975bf-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="975bf-117">Optional query parameters</span></span>
<span data-ttu-id="975bf-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="975bf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="975bf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="975bf-119">Request headers</span></span>
| <span data-ttu-id="975bf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="975bf-120">Name</span></span>      |<span data-ttu-id="975bf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="975bf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="975bf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="975bf-122">Authorization</span></span>  | <span data-ttu-id="975bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="975bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="975bf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="975bf-125">Request body</span></span>
<span data-ttu-id="975bf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="975bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="975bf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="975bf-127">Response</span></span>

<span data-ttu-id="975bf-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="975bf-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="975bf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="975bf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="975bf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="975bf-130">Request</span></span>
<span data-ttu-id="975bf-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="975bf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="975bf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="975bf-132">Response</span></span>
<span data-ttu-id="975bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="975bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="975bf-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="975bf-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="975bf-137">Basic</span><span class="sxs-lookup"><span data-stu-id="975bf-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mastercategories-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="975bf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="975bf-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mastercategories-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookuser-list-mastercategories.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-list-mastercategories.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
