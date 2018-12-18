---
title: Listar TableColumnCollection
description: Recupere uma lista de objetos tablecolumn.
author: lumine2008
ms.openlocfilehash: b050d9e322df9aa6f6a07d509ccf7a17637e77e6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309538"
---
# <a name="list-tablecolumncollection"></a><span data-ttu-id="71bf6-103">Listar TableColumnCollection</span><span class="sxs-lookup"><span data-stu-id="71bf6-103">List TableColumnCollection</span></span>

<span data-ttu-id="71bf6-104">Recupere uma lista de objetos tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="71bf6-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="71bf6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="71bf6-105">Permissions</span></span>
<span data-ttu-id="71bf6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71bf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71bf6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71bf6-108">Permission type</span></span>      | <span data-ttu-id="71bf6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71bf6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71bf6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71bf6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71bf6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71bf6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71bf6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71bf6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71bf6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71bf6-113">Not supported.</span></span>    |
|<span data-ttu-id="71bf6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71bf6-114">Application</span></span> | <span data-ttu-id="71bf6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71bf6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71bf6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71bf6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71bf6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71bf6-117">Optional query parameters</span></span>
<span data-ttu-id="71bf6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71bf6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71bf6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71bf6-119">Request headers</span></span>
| <span data-ttu-id="71bf6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="71bf6-120">Name</span></span>      |<span data-ttu-id="71bf6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="71bf6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71bf6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71bf6-122">Authorization</span></span>  | <span data-ttu-id="71bf6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71bf6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71bf6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71bf6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="71bf6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="71bf6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71bf6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71bf6-128">Request body</span></span>
<span data-ttu-id="71bf6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71bf6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71bf6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="71bf6-130">Response</span></span>

<span data-ttu-id="71bf6-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [WorkbookTableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71bf6-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71bf6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71bf6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71bf6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71bf6-133">Request</span></span>
<span data-ttu-id="71bf6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71bf6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
##### <a name="response"></a><span data-ttu-id="71bf6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="71bf6-135">Response</span></span>
<span data-ttu-id="71bf6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71bf6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->