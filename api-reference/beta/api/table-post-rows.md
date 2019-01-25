---
title: Criar TableRow
description: 'Adiciona linhas até o final da tabela. Observe que a API pode aceitar os dados de várias linhas usando essa API. Adicionar uma linha por vez pode levar à redução de desempenho. A abordagem recomendada seria as linhas juntos em uma única chamada em vez de fazer a inserção de linha única de lote. Para obter melhores resultados, coletado linhas a ser inserido no lado do aplicativo e realizar linhas única Adicionar operação. Experimentar o número de linhas para determinar o número ideal de linhas para usar em única chamada de API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 88fd78516528f62925b18c1c45d9452404be6881
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529506"
---
# <a name="create-tablerow"></a>Criar TableRow

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adiciona linhas até o final da tabela. Observe que a API pode aceitar os dados de várias linhas usando essa API. Adicionar uma linha por vez pode levar à redução de desempenho. A abordagem recomendada seria as linhas juntos em uma única chamada em vez de fazer a inserção de linha única de lote. Para obter melhores resultados, coletado linhas a ser inserido no lado do aplicativo e realizar linhas única Adicionar operação. Experimentar o número de linhas para determinar o número ideal de linhas para usar em única chamada de API. 

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
|índice|number|Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.|
|values|(booliano, cadeia de caracteres ou número)|Uma matriz de 2-dimensional dos valores não formatados das linhas da tabela.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.

## <a name="example"></a>Exemplo
Neste exemplo, duas linhas de dados são inseridas no fim da tabela. 

##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-post-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
