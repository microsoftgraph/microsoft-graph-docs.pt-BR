---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: bd3c1a2b1cbfcb8d0e47f9d7ec93b0695e9854c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870235"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="4c049-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="4c049-103">TableColumnCollection: add</span></span>

> <span data-ttu-id="4c049-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c049-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c049-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c049-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c049-106">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="4c049-106">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c049-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c049-107">Permissions</span></span>
<span data-ttu-id="4c049-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c049-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c049-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c049-110">Permission type</span></span>      | <span data-ttu-id="4c049-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c049-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c049-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c049-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c049-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c049-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4c049-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c049-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c049-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c049-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4c049-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c049-116">Application</span></span> | <span data-ttu-id="4c049-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c049-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c049-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c049-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="4c049-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c049-119">Request headers</span></span>
| <span data-ttu-id="4c049-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4c049-120">Name</span></span>       | <span data-ttu-id="4c049-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c049-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4c049-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c049-122">Authorization</span></span>  | <span data-ttu-id="4c049-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c049-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c049-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4c049-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4c049-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4c049-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c049-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c049-128">Request body</span></span>
<span data-ttu-id="4c049-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c049-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c049-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4c049-130">Parameter</span></span>    | <span data-ttu-id="4c049-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c049-131">Type</span></span>   |<span data-ttu-id="4c049-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c049-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c049-133">índice</span><span class="sxs-lookup"><span data-stu-id="4c049-133">index</span></span>|<span data-ttu-id="4c049-134">number</span><span class="sxs-lookup"><span data-stu-id="4c049-134">number</span></span>|<span data-ttu-id="4c049-p105">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="4c049-p105">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="4c049-139">values</span><span class="sxs-lookup"><span data-stu-id="4c049-139">values</span></span>|<span data-ttu-id="4c049-140">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="4c049-140">(boolean or string or number)</span></span>|<span data-ttu-id="4c049-p106">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="4c049-p106">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="4c049-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c049-143">Response</span></span>

<span data-ttu-id="4c049-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c049-144">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c049-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c049-145">Example</span></span>
<span data-ttu-id="4c049-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4c049-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4c049-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c049-147">Request</span></span>
<span data-ttu-id="4c049-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c049-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="4c049-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c049-149">Response</span></span>
<span data-ttu-id="4c049-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c049-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
