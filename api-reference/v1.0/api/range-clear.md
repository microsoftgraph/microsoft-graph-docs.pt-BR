---
title: 'Range: clear'
description: Limpa valores de intervalo, formatação, preenchimento, borda, etc.
localization_priority: Normal
ms.openlocfilehash: 8bf7bafd42947528c98a83819afd7b16f49d2e7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861912"
---
# <a name="range-clear"></a>Range: clear

Limpa valores de intervalo, formatação, preenchimento, borda, etc.
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
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

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
|applyTo|string|Opcional. Determina o tipo de ação clara.  Os valores possíveis são: `All`, `Formats`, `Contents`.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
