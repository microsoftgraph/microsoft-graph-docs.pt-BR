---
title: 'Chart: Image'
description: Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c9a3eb3c23e7222a083eb6e34f5e08be44424250
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575697"
---
# <a name="chart-image"></a>Chart: Image

Namespace: microsoft.graph

Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "samples" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Workbook-Session-Id  | ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.|

## <a name="path-parameters"></a>Parâmetros do caminho
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|height|Int32|A altura desejada da imagem resultante. Opcional.|
|width|Int32|A largura desejada da imagem resultante. Opcional.|
|fittingMode|string|O método usado para dimensionar o gráfico para as dimensões especificadas (se a altura e a largura estão definidas)."  Os valores possíveis são: `Fit`, `FitAndCenter`, `Fill`.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.

##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a>Uso

Você pode exibir a cadeia de caracteres de Base 64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.

Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`. Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste. Esta é a aparência da imagem de gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

