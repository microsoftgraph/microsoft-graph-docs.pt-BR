---
title: tipo de recurso da pasta de trabalho
description: Contém objetos de pasta de trabalho relacionados, como planilhas, tabelas, intervalos e assim por diante.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 69d04f6ccd5e537c97854abcb1cf2a9c24820a87
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575704"
---
# <a name="workbook-resource-type"></a>tipo de recurso da pasta de trabalho

Namespace: microsoft.graph

Contém objetos de pasta de trabalho relacionados, como planilhas, tabelas, intervalos e assim por diante.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar sessão](../api/workbook-createsession.md) | [workbookSessionInfo](workbooksessioninfo.md) |Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.|
|[Fechar sessão](../api/workbook-closesession.md) | Nenhum(a) |Fechar uma sessão existente.|
|[Atualizar sessão](../api/workbook-refreshsession.md) | Nenhum(a) |Atualizar uma sessão existente.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|names|coleção [workbookNamedItem](workbooknameditem.md) |Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.|
|tables|coleção [WorkbookTable](workbooktable.md) |Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.|
|worksheets|coleção [WorkbookWorksheet](workbookworksheet.md) |Representa uma coleção de planilhas associadas à pasta de trabalho. Somente leitura.|
|workbbookApplication|[workbookApplication](workbookapplication.md) |Representa a workbookApplication do Excel que gerencia a planilha.|
|operações|coleção [workbookOperation](workbookoperation.md)|O status das operações da Workbook. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status de uma operação de longa execução se o cabeçalho `Location` retornar na resposta. Somente leitura. Anulável.|

## <a name="functions"></a>Funções

[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /me/drive/root/workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função. O valor `error` de `null` indica a execução bem-sucedida da função. 

A lista completa de funções com suporte está listada [aqui](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.

_Observações importantes:_ 
* O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.  
* O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs. 

Exemplo: **vlookup**

Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:

1. O valor que você deseja pesquisar, também chamado de valor de pesquisa.
2. O intervalo em que o valor de pesquisa está localizado. Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna no intervalo para que o PROCV funcione corretamente. Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deve começar com C.
3. O número da coluna no intervalo que contém o valor de retorno. Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.
4. Opcionalmente, você pode especificar TRUE se desejar uma correspondência aproximada ou FALSE se desejar uma correspondência exata do valor de retorno. Se você não especificar nada, o valor padrão sempre será TRUE ou uma correspondência aproximada.

Dentro de uma célula, a função `vlookup` tem esta aparência: 

= PROCV(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor de retorno, opcionalmente, TRUE para coincidência aproximada ou FALSE para uma correspondência exata)

(Confira a documentação para a função do Excel [PROCV](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)).

O exemplo abaixo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.
Solicitação: 

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

Resposta:

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

Exemplo: `median`

Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.

Dentro de uma célula, a função `median` se parece com este exemplo:

=MED(A2:A6)

(Confira a documentação para a função [MED](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)).

O exemplo abaixo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel. 

Solicitação: 

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

Resposta:

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
## <a name="json-representation"></a>Representação JSON

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.workbook"
}-->
``` json
{
    "id": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


