---
author: JeremyKelley
title: Obter listItem
description: Retorna os metadados de um item em uma lista do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 22e7ea8cf90cb1677ddcfa653d9e2c67ce3786c7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238768"
---
# <a name="get-listitem"></a><span data-ttu-id="b96ca-103">Obter listItem</span><span class="sxs-lookup"><span data-stu-id="b96ca-103">Get listItem</span></span>

<span data-ttu-id="b96ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b96ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b96ca-105">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="b96ca-105">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="b96ca-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b96ca-108">Permissions</span></span>

<span data-ttu-id="b96ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b96ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b96ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b96ca-111">Permission type</span></span>      | <span data-ttu-id="b96ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b96ca-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b96ca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b96ca-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b96ca-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b96ca-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b96ca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b96ca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b96ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b96ca-116">Not supported.</span></span>    |
|<span data-ttu-id="b96ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b96ca-117">Application</span></span> | <span data-ttu-id="b96ca-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b96ca-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span></span> |

> <span data-ttu-id="b96ca-119">**Observação**: a permissão do aplicativo Sites.Manage.All será necessária se a lista do SharePoint tiver as configurações de aprovação de conteúdo ativadas.</span><span class="sxs-lookup"><span data-stu-id="b96ca-119">**Note**: The application permission Sites.Manage.All is required if the SharePoint list has content approval settings turned on.</span></span> <span data-ttu-id="b96ca-120">Caso contrário, o Microsoft Graph não recuperará os itens da lista que têm um status de aprovação diferente de Aprovado.</span><span class="sxs-lookup"><span data-stu-id="b96ca-120">Otherwise, Microsoft Graph won't retrieve  list items that have an approval status other than Approved.</span></span>

## <a name="http-request"></a><span data-ttu-id="b96ca-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b96ca-121">HTTP request</span></span>

<span data-ttu-id="b96ca-122">Obter um listItem</span><span class="sxs-lookup"><span data-stu-id="b96ca-122">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="b96ca-123">Obter os valores de coluna de um listItem</span><span class="sxs-lookup"><span data-stu-id="b96ca-123">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="b96ca-124">Obter valores de coluna específicos de um listItem</span><span class="sxs-lookup"><span data-stu-id="b96ca-124">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b96ca-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b96ca-125">Optional query parameters</span></span>
<span data-ttu-id="b96ca-126">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b96ca-126">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b96ca-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b96ca-127">Request headers</span></span>

| <span data-ttu-id="b96ca-128">Nome</span><span class="sxs-lookup"><span data-stu-id="b96ca-128">Name</span></span>      |<span data-ttu-id="b96ca-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b96ca-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b96ca-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b96ca-130">Authorization</span></span>  | <span data-ttu-id="b96ca-131">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="b96ca-131">Bearer {code}.</span></span> <span data-ttu-id="b96ca-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b96ca-132">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b96ca-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b96ca-133">Request body</span></span>

<span data-ttu-id="b96ca-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b96ca-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b96ca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b96ca-135">Response</span></span> 

<span data-ttu-id="b96ca-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um [item][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b96ca-136">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b96ca-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b96ca-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b96ca-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b96ca-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b96ca-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b96ca-139">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="b96ca-140">C#</span><span class="sxs-lookup"><span data-stu-id="b96ca-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b96ca-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b96ca-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b96ca-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b96ca-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b96ca-143">Java</span><span class="sxs-lookup"><span data-stu-id="b96ca-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b96ca-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b96ca-144">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
} -->

