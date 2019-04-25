---
title: Listar linhas
description: Recupere uma lista de objetos tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 46d121e1555cad780d12fa6922d6aa3867cc792e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536737"
---
# <a name="list-rows"></a><span data-ttu-id="10205-103">Listar linhas</span><span class="sxs-lookup"><span data-stu-id="10205-103">List rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10205-104">Recupere uma lista de objetos tablerow.</span><span class="sxs-lookup"><span data-stu-id="10205-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="10205-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="10205-105">Permissions</span></span>
<span data-ttu-id="10205-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10205-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10205-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10205-108">Permission type</span></span>      | <span data-ttu-id="10205-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10205-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10205-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10205-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10205-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10205-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10205-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10205-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10205-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10205-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10205-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10205-114">Application</span></span> | <span data-ttu-id="10205-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10205-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10205-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10205-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10205-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10205-117">Optional query parameters</span></span>
<span data-ttu-id="10205-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10205-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="10205-119">Para resultados confiáveis, use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="10205-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="10205-120">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="10205-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10205-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10205-121">Request headers</span></span>
| <span data-ttu-id="10205-122">Nome</span><span class="sxs-lookup"><span data-stu-id="10205-122">Name</span></span>      |<span data-ttu-id="10205-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="10205-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10205-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="10205-124">Authorization</span></span>  | <span data-ttu-id="10205-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10205-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10205-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="10205-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="10205-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="10205-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10205-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10205-130">Request body</span></span>
<span data-ttu-id="10205-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10205-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10205-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="10205-132">Response</span></span>

<span data-ttu-id="10205-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10205-133">If successful, this method returns a `200 OK` response code and collection of [TableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10205-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10205-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10205-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10205-135">Request</span></span>
<span data-ttu-id="10205-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10205-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="10205-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="10205-137">Response</span></span>
<span data-ttu-id="10205-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10205-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="10205-141">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar por um grande número de linhas.</span><span class="sxs-lookup"><span data-stu-id="10205-141">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="10205-142">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="10205-142">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
