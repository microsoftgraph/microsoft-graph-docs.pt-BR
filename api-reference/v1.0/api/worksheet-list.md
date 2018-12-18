---
title: Listar WorksheetCollection
description: Recupere uma lista de objetos de planilha.
author: lumine2008
ms.openlocfilehash: 1680a7abce783d4b1954c9bb05e03627d57a3783
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351132"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="a27ce-103">Listar WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="a27ce-103">List WorksheetCollection</span></span>

<span data-ttu-id="a27ce-104">Recupere uma lista de objetos de planilha.</span><span class="sxs-lookup"><span data-stu-id="a27ce-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a27ce-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a27ce-105">Permissions</span></span>
<span data-ttu-id="a27ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a27ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a27ce-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a27ce-108">Permission type</span></span>      | <span data-ttu-id="a27ce-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a27ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a27ce-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a27ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a27ce-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a27ce-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a27ce-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a27ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a27ce-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a27ce-113">Not supported.</span></span>    |
|<span data-ttu-id="a27ce-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a27ce-114">Application</span></span> | <span data-ttu-id="a27ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a27ce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a27ce-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a27ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a27ce-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a27ce-117">Optional query parameters</span></span>
<span data-ttu-id="a27ce-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a27ce-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a27ce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a27ce-119">Request headers</span></span>
| <span data-ttu-id="a27ce-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a27ce-120">Name</span></span>      |<span data-ttu-id="a27ce-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a27ce-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a27ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a27ce-122">Authorization</span></span>  | <span data-ttu-id="a27ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a27ce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a27ce-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a27ce-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a27ce-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a27ce-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a27ce-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a27ce-128">Request body</span></span>
<span data-ttu-id="a27ce-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a27ce-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a27ce-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27ce-130">Response</span></span>

<span data-ttu-id="a27ce-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a27ce-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a27ce-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a27ce-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a27ce-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a27ce-133">Request</span></span>
<span data-ttu-id="a27ce-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a27ce-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="a27ce-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27ce-135">Response</span></span>
<span data-ttu-id="a27ce-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a27ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->