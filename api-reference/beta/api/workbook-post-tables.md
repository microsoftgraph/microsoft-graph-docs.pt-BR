---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2e8f2d10c36ec8e2737b77b69fec46a4dd65e50c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448505"
---
# <a name="create-table"></a>Criar tabela

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use essa API para criar uma nova tabela.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Workbook-Session-Id  | ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro           | Tipo      |Descrição|
|:---------------|:----------|:----------|
| Endereço  | string| Endereço do intervalo. Se você estiver chamando esta API fora do `worksheets/{id or name}/tables/add` caminho, não será necessário para o prefixo do nome da planilha no endereço. No entanto, se você estiver ligando para `workbook/tables/add` fora do caminho, forneça o nome da planilha na qual a tabela precisa ser criada (exemplo `sheet1!A1:D4`:)|
| hasHeaders  | booliano|Valor booliano que indica se o intervalo tem rótulos de coluna. Se a fonte não contiver cabeçalhos (ou seja,. Quando essa propriedade for definida como false, o Excel gerará automaticamente o cabeçalho deslocando os dados de uma linha para baixo.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbooktable](../resources/workbooktable.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-workbook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-workbook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-workbook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
