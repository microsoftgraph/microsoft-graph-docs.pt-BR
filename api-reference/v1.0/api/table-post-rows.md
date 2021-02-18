---
title: Criar TableRow
description: 'Adiciona linhas ao final da tabela. Observe que a API pode aceitar vários dados de linhas usando essa API. Adicionar uma linha por vez pode levar à degradação do desempenho. A abordagem recomendada seria reunir as linhas em lote em uma única chamada em vez de fazer a inserção de uma única linha. Para melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e execute uma única operação de aplicação de linhas. Experimente o número de linhas para determinar o número ideal de linhas a ser usado em uma única chamada à API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 69f80f8b0391102d6501d2481c3377d899003e6b
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292298"
---
# <a name="create-tablerow"></a>Criar TableRow

Namespace: microsoft.graph

Adiciona linhas ao final da tabela. Observe que a API pode aceitar vários dados de linhas usando essa API. Adicionar uma linha por vez pode levar à degradação do desempenho. A abordagem recomendada seria reunir as linhas em lote em uma única chamada em vez de fazer a inserção de uma única linha. Para melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e execute uma única operação de aplicação de linhas. Experimente o número de linhas para determinar o número ideal de linhas a ser usado em uma única chamada à API. 

## <a name="error-handling"></a>Tratamento de erros

Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504. A resposta apropriada para esta mensagem de erro é repetir a solicitação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Workbook-Session-Id  | ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|index|number|Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.|
|values|Json|Uma matriz bidimensional de valores não formatados das linhas da tabela (booliana, cadeia de caracteres ou número).|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.

## <a name="example"></a>Exemplo
Neste exemplo, duas linhas de dados são inseridas no final da tabela. 

##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->

