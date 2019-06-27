---
title: 'Chart: setPosition'
description: Posiciona o gráfico em relação às células na planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1baff92660d445c8c2d578db6a5b0ee63b863ca8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261919"
---
# <a name="chart-setposition"></a>Chart: setPosition

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Posiciona o gráfico em relação às células na planilha.
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
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

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
|startCell|string|A célula inicial. Esse é o local para o qual o gráfico será movido. A célula inicial é a célula superior esquerda ou direita, dependendo das configurações de exibição do usuário, da esquerda para a direita.|
|endCell|string|Opcional. A célula final. Quando é especificada, a altura e a largura do gráfico são definidas para cobrirem totalmente essa célula ou intervalo.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/chart_setposition-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/chart_setposition-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chart_setposition-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
