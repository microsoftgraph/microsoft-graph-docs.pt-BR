---
title: Listar TableCollection
description: Recupere uma lista de objetos de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 296fac43d0aa415effd35f4477994bd38763cf86
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642048"
---
# <a name="list-tablecollection"></a><span data-ttu-id="69ce0-103">Listar TableCollection</span><span class="sxs-lookup"><span data-stu-id="69ce0-103">List TableCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69ce0-104">Recupere uma lista de objetos de tabela.</span><span class="sxs-lookup"><span data-stu-id="69ce0-104">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="69ce0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="69ce0-105">Permissions</span></span>
<span data-ttu-id="69ce0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ce0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ce0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69ce0-108">Permission type</span></span>      | <span data-ttu-id="69ce0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69ce0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69ce0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69ce0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69ce0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69ce0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="69ce0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69ce0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69ce0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69ce0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="69ce0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69ce0-114">Application</span></span> | <span data-ttu-id="69ce0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69ce0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69ce0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69ce0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69ce0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="69ce0-117">Optional query parameters</span></span>
<span data-ttu-id="69ce0-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="69ce0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69ce0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69ce0-119">Request headers</span></span>
| <span data-ttu-id="69ce0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="69ce0-120">Name</span></span>      |<span data-ttu-id="69ce0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="69ce0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="69ce0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="69ce0-122">Authorization</span></span>  | <span data-ttu-id="69ce0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69ce0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69ce0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="69ce0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="69ce0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="69ce0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ce0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69ce0-128">Request body</span></span>
<span data-ttu-id="69ce0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69ce0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69ce0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ce0-130">Response</span></span>

<span data-ttu-id="69ce0-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69ce0-131">If successful, this method returns a `200 OK` response code and collection of [Table](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69ce0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69ce0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69ce0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69ce0-133">Request</span></span>
<span data-ttu-id="69ce0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69ce0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="69ce0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ce0-135">Response</span></span>
<span data-ttu-id="69ce0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69ce0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
