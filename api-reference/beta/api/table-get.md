---
title: Obter tabela
description: Recupere as propriedades e os relacionamentos do objeto de tabela.
author: lumine2008
ms.openlocfilehash: 9bac729dc25b9433f5af1491be275e6a2ac47f22
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360316"
---
# <a name="get-table"></a><span data-ttu-id="f2012-103">Obter tabela</span><span class="sxs-lookup"><span data-stu-id="f2012-103">Get Table</span></span>

> <span data-ttu-id="f2012-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2012-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2012-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2012-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2012-106">Recupere as propriedades e os relacionamentos do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="f2012-106">Retrieve the properties and relationships of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2012-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2012-107">Permissions</span></span>
<span data-ttu-id="f2012-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2012-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2012-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2012-110">Permission type</span></span>      | <span data-ttu-id="f2012-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2012-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2012-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2012-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2012-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2012-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2012-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2012-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2012-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2012-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2012-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2012-116">Application</span></span> | <span data-ttu-id="f2012-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2012-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2012-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2012-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2012-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2012-119">Optional query parameters</span></span>
<span data-ttu-id="f2012-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2012-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2012-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2012-121">Request headers</span></span>
| <span data-ttu-id="f2012-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f2012-122">Name</span></span>      |<span data-ttu-id="f2012-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2012-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2012-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2012-124">Authorization</span></span>  | <span data-ttu-id="f2012-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2012-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2012-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f2012-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="f2012-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f2012-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2012-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2012-130">Request body</span></span>
<span data-ttu-id="f2012-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2012-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2012-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2012-132">Response</span></span>

<span data-ttu-id="f2012-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2012-133">If successful, this method returns a `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2012-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2012-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2012-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2012-135">Request</span></span>
<span data-ttu-id="f2012-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2012-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_table"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
```
##### <a name="response"></a><span data-ttu-id="f2012-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2012-137">Response</span></span>
<span data-ttu-id="f2012-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2012-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
