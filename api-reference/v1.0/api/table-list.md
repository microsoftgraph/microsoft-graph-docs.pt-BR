---
title: Listar TableCollection
description: Recupere uma lista de objetos de tabela.
ms.openlocfilehash: 56864105d199b461b14e66543f683e1815b28021
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004073"
---
# <a name="list-tablecollection"></a><span data-ttu-id="ca6f2-103">Listar TableCollection</span><span class="sxs-lookup"><span data-stu-id="ca6f2-103">List TableCollection</span></span>

<span data-ttu-id="ca6f2-104">Recupere uma lista de objetos de tabela.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-104">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca6f2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca6f2-105">Permissions</span></span>
<span data-ttu-id="ca6f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca6f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca6f2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca6f2-108">Permission type</span></span>      | <span data-ttu-id="ca6f2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca6f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca6f2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca6f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ca6f2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca6f2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca6f2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca6f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca6f2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-113">Not supported.</span></span>    |
|<span data-ttu-id="ca6f2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca6f2-114">Application</span></span> | <span data-ttu-id="ca6f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca6f2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca6f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca6f2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ca6f2-117">Optional query parameters</span></span>
<span data-ttu-id="ca6f2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca6f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6f2-119">Request headers</span></span>
| <span data-ttu-id="ca6f2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ca6f2-120">Name</span></span>      |<span data-ttu-id="ca6f2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca6f2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca6f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca6f2-122">Authorization</span></span>  | <span data-ttu-id="ca6f2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca6f2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ca6f2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ca6f2-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca6f2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6f2-128">Request body</span></span>
<span data-ttu-id="ca6f2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca6f2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6f2-130">Response</span></span>

<span data-ttu-id="ca6f2-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [WorkbookTable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTable](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca6f2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca6f2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca6f2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6f2-133">Request</span></span>
<span data-ttu-id="ca6f2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="ca6f2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6f2-135">Response</span></span>
<span data-ttu-id="ca6f2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
> <span data-ttu-id="ca6f2-139">**Observação:** use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) para navegar por um grande número de tabelas.</span><span class="sxs-lookup"><span data-stu-id="ca6f2-139">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) query parameters to page through large numbers of tables.</span></span>

<span data-ttu-id="ca6f2-140">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="ca6f2-140">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
