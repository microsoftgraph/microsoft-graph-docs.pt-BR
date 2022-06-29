---
title: Usar funções de pasta de trabalho no Excel
description: Você pode usar as funções de pasta de trabalho no Excel com o Microsoft Graph para invocar qualquer função de pasta de trabalho. Inclui exemplos para funções de procv e mediana.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: eec1834a63ab87304b33eea1f75629fe12e56aec
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443365"
---
# <a name="use-workbook-functions-in-excel"></a>Usar funções de pasta de trabalho no Excel

Você pode usar as funções de pasta de trabalho no Excel com o Microsoft Graph para invocar qualquer função de pasta de trabalho usando a seguinte sintaxe: `POST /me/drive/root/workbook/functions/{function-name}`. Você fornece os argumentos de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função. O valor `error` de `null` indica a execução bem-sucedida da função.

Para obter uma lista completa das funções com suporte, consulte [a classe Excel.Functions](/javascript/api/excel/excel.functions?view=excel-js-preview&preserve-view=true). Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.

> [!IMPORTANT]
> - O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.  
> - O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs.

## <a name="example-vlookup"></a>Exemplo: `vlookup`

Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:

- **lookup_value** (obrigatório): o valor que você deseja pesquisar.

- **table_array** (obrigatório): o intervalo de células em que o valor de pesquisa está localizado. Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna do intervalo para **que PROCV** funcione corretamente. Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deverá começar com C.

- **col_index_num** (obrigatório): o número da coluna no intervalo que contém o valor retornado. Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.

- **range_lookup** (opcional): o valor lógico que especifica se você deseja que **PROCV** localize uma correspondência aproximada ou exata. Especifique **VERDADEIRO** se desejar uma correspondência aproximada ou **FALSO** se desejar uma correspondência exata do valor de retorno. Se você não especificar nada, o valor padrão sempre será VERDADEIRO ou uma correspondência aproximada.

Dentro de uma célula, a função `vlookup` tem esta aparência:

`=VLOOKUP`(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor retornado, opcionalmente especifique TRUE para correspondência aproximada ou FALSE para uma correspondência exata)

Para obter mais informações, consulte a documentação da [função Excel PROCV](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).

### <a name="request"></a>Solicitação

O seguinte exemplo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

### <a name="response"></a>Resposta

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

## <a name="example-median"></a>Exemplo: `median`

Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.

Dentro de uma célula, a função `median` se parece com este exemplo:

`=MEDIAN(A2:A6)`

Para obter mais informações, consulte a documentação da [função MEDIAN do Excel](https://support.office.com/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).

### <a name="request"></a>Solicitação

O seguinte exemplo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel.

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ]
}
```

### <a name="response"></a>Resposta

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

## <a name="see-also"></a>Confira também

* [Gerenciar sessões do Excel usando o Microsoft Graph](excel-manage-sessions.md)
* [Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph](excel-write-to-workbook.md)
* [Atualizar um formato de intervalo no Excel com o Microsoft Graph](excel-update-range-format.md)
* [Exibir uma imagem do gráfico do Excel com o Microsoft Graph](excel-display-chart-image.md)
* [Usar a API REST do Excel](/graph/api/resources/excel)
