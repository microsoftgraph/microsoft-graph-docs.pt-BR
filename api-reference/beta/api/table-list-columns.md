---
title: Listar colunas
description: Recupere uma lista de objetos tablecolumn.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 69577701a2bd94bea50fa7619dc8c3261f4458d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876325"
---
# <a name="list-columns"></a><span data-ttu-id="e8b68-103">Listar colunas</span><span class="sxs-lookup"><span data-stu-id="e8b68-103">List columns</span></span>

> <span data-ttu-id="e8b68-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8b68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8b68-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8b68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8b68-106">Recupere uma lista de objetos tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="e8b68-106">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8b68-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8b68-107">Permissions</span></span>
<span data-ttu-id="e8b68-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8b68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8b68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8b68-110">Permission type</span></span>      | <span data-ttu-id="e8b68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8b68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8b68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8b68-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8b68-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8b68-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8b68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8b68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8b68-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8b68-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8b68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8b68-116">Application</span></span> | <span data-ttu-id="e8b68-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8b68-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8b68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8b68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8b68-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8b68-119">Optional query parameters</span></span>
<span data-ttu-id="e8b68-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b68-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="e8b68-121">Para resultados confiáveis, use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="e8b68-121">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="e8b68-122">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="e8b68-122">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8b68-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b68-123">Request headers</span></span>
| <span data-ttu-id="e8b68-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e8b68-124">Name</span></span>      |<span data-ttu-id="e8b68-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8b68-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8b68-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8b68-126">Authorization</span></span>  | <span data-ttu-id="e8b68-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8b68-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8b68-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e8b68-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8b68-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e8b68-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8b68-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b68-132">Request body</span></span>
<span data-ttu-id="e8b68-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8b68-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8b68-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b68-134">Response</span></span>

<span data-ttu-id="e8b68-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b68-135">If successful, this method returns a `200 OK` response code and collection of [TableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8b68-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8b68-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8b68-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b68-137">Request</span></span>
<span data-ttu-id="e8b68-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8b68-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="e8b68-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b68-139">Response</span></span>
<span data-ttu-id="e8b68-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8b68-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="e8b68-143">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar por um grande número de colunas.</span><span class="sxs-lookup"><span data-stu-id="e8b68-143">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="e8b68-144">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="e8b68-144">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
