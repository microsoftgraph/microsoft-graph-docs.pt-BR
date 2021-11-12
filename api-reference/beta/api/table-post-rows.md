---
title: Criar tableRow
description: Adicione linhas ao final de uma tabela.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4b04288f2c054a81f30f2923cc7fd92901cf4d63
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60939194"
---
# <a name="create-tablerow"></a>Criar tableRow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione linhas ao final de uma tabela. 

Observe que a API pode aceitar dados de várias linhas usando essa API. Adicionar uma linha por vez pode levar à degradação do desempenho. A abordagem recomendada é reunir as linhas em lotes em uma única chamada em vez de fazer a inserção de linha única. Para melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e execute uma única operação de aplicação de linha. Experimente o número de linhas para determinar o número ideal de linhas a ser usado em uma única chamada de API. 

Essa solicitação pode resultar ocasionalmente em um `504 HTTP` erro. A resposta apropriada para esta mensagem de erro é repetir a solicitação.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows
POST /me/drive/root:/{item-path}:/workbookworksheets/{id|name}/tables/{id|name}/rows
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type | application/json. Obrigatório.|
| Preferir  | respond-async. Indica que a solicitação é uma solicitação assíncrona. Opcional.  |
| Workbook-Session-Id  | {Workbook-Session-Id}. Criado a partir **da solicitação createSession.** Opcional.|

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

|Parâmetro|Tipo|Descrição|
|:---------------|:--------|:----------|
| índice| Int32| Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.|
| values| [Json](../resources/json.md)| Uma matriz bidimensional de valores não formatados das linhas de tabela.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto workbookTableRow](../resources/workbooktablerow.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-two-rows-to-a-table"></a>Exemplo 1: Adicionar duas linhas a uma tabela

Neste exemplo, duas linhas de dados são inseridas no final da tabela. 

#### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "Table1"],
  "name": "tablerowcollection_add_1"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows
Content-type: application/json

{
  "values": "[
    [1, 2, 3],
    [4, 5, 6]
  ]"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-add-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerowcollection-add-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "index": 99,
  "values": "[[1, 2, 3]]"
}
```

### <a name="example-2-add-two-rows-to-a-table-asynchronously"></a>Exemplo 2: Adicionar duas linhas a uma tabela de forma assíncrona

As solicitações assíncrona serão úteis se a solicitação levar mais tempo do que o esperado. Observe que `Workbook-Session-Id` o header é necessário na emissão de solicitações assíncronas. O usuário precisa criar [sessão antes](./workbook-createsession.md) de usar recursos de API avançados assíncrono. O header `Prefer:respond-async` também é necessário nas solicitações assíncrona.

Para recursos assíncrono, o usuário geralmente precisa emitir solicitações de 2 a 3. Esta solicitação, [Obter solicitação workbookOperation](./workbookoperation-get.md) e, opcionalmente, [Obter solicitação tableRowOperationResult.](./workbook-tablerowoperationresult.md)

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação assíncrona. Observe que `202 Accepted` isso só acontecerá quando a solicitação levar muito tempo para responder. Se a solicitação for concluída rapidamente, ela funcionará como uma solicitação de sincronização regular, voltando ao [Exemplo 1](#example-1-add-two-rows-to-a-table).


<!-- {
  "blockType": "request",
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "Table1"],
  "name": "tablerowcollection_add_1"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows
Content-type: application/json
Prefer: respond-async
Workbook-Session-Id: {Workbook-Session-Id}

{
  "values": "[
    [1, 2, 3],
    [4, 5, 6]
  ]"
}
```

#### <a name="response"></a>Resposta

Aqui está outro exemplo da resposta que levará a uma operação assíncrona. Para obter detalhes, [consulte Get workbookOperation and](./workbookoperation-get.md) Get [tableRowOperationResult](./workbook-tablerowoperationresult.md).
<!-- {
  "blockType": "response",
  "truncated": true,
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "0195cfac-bd22-4f91-b276-dece0aa2378b", "Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ=="],
  "@odata.type": "microsoft.graph.Json"
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/operations/0195cfac-bd22-4f91-b276-dece0aa2378b?sessionId=Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ==
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
