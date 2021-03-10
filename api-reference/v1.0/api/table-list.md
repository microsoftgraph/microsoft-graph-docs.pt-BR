---
title: Listar TableCollection
description: Recupere uma lista de objetos de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f93bd8cf72d66e283554b619a635ac0f6e59523d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575564"
---
# <a name="list-tablecollection"></a><span data-ttu-id="4cd14-103">Listar TableCollection</span><span class="sxs-lookup"><span data-stu-id="4cd14-103">List TableCollection</span></span>

<span data-ttu-id="4cd14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cd14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cd14-105">Recupere uma lista de objetos de tabela.</span><span class="sxs-lookup"><span data-stu-id="4cd14-105">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cd14-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4cd14-106">Permissions</span></span>
<span data-ttu-id="4cd14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cd14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cd14-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cd14-109">Permission type</span></span>      | <span data-ttu-id="4cd14-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cd14-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cd14-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cd14-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4cd14-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cd14-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4cd14-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cd14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cd14-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cd14-114">Not supported.</span></span>    |
|<span data-ttu-id="4cd14-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cd14-115">Application</span></span> | <span data-ttu-id="4cd14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cd14-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cd14-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cd14-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables
GET /me/drive/root:/{item-path}:/workbook/tables
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4cd14-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4cd14-118">Optional query parameters</span></span>
<span data-ttu-id="4cd14-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4cd14-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cd14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cd14-120">Request headers</span></span>
| <span data-ttu-id="4cd14-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4cd14-121">Name</span></span>      |<span data-ttu-id="4cd14-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cd14-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4cd14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cd14-123">Authorization</span></span>  | <span data-ttu-id="4cd14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cd14-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cd14-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4cd14-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="4cd14-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4cd14-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cd14-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cd14-129">Request body</span></span>
<span data-ttu-id="4cd14-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4cd14-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cd14-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cd14-131">Response</span></span>

<span data-ttu-id="4cd14-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [WorkbookTable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cd14-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookTable](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4cd14-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cd14-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cd14-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cd14-134">Request</span></span>
<span data-ttu-id="4cd14-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cd14-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4cd14-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cd14-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
# <a name="c"></a>[<span data-ttu-id="4cd14-137">C#</span><span class="sxs-lookup"><span data-stu-id="4cd14-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cd14-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cd14-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cd14-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cd14-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4cd14-140">Java</span><span class="sxs-lookup"><span data-stu-id="4cd14-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4cd14-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cd14-141">Response</span></span>
<span data-ttu-id="4cd14-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cd14-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
> <span data-ttu-id="4cd14-145">**Observação:** use os parâmetros de consulta [$top](/graph/query-parameters#top) e [$skip](/graph/query-parameters#top) para navegar por um grande número de tabelas.</span><span class="sxs-lookup"><span data-stu-id="4cd14-145">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#top) query parameters to page through large numbers of tables.</span></span>

<span data-ttu-id="4cd14-146">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="4cd14-146">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
