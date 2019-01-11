---
title: Tipo de recurso de pasta de trabalho
description: A pasta de trabalho é o objeto de nível superior que inclui os objetos workbook relacionados, como planilhas, tabelas, intervalos, etc.
localization_priority: Priority
ms.openlocfilehash: 25b74bcc0ce0b54aace11ed9f829435a510f9c9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835417"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="7ebd2-103">Tipo de recurso de pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="7ebd2-103">Workbook resource type</span></span>

<span data-ttu-id="7ebd2-104">A pasta de trabalho é o objeto de nível superior que inclui os objetos workbook relacionados, como planilhas, tabelas, intervalos, etc.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-104">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ebd2-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ebd2-105">JSON representation</span></span>

<span data-ttu-id="7ebd2-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7ebd2-106">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbook"
}-->

```json
{
  "names": [{"@odata.type": "microsoft.graph.workbookNamedItem"}],
  "tables": [{"@odata.type": "microsoft.graph.workbookTable"}],
  "worksheets": [{"@odata.type": "microsoft.graph.workbookWorksheet"}]
}
```

## <a name="properties"></a><span data-ttu-id="7ebd2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ebd2-107">Properties</span></span>
<span data-ttu-id="7ebd2-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ebd2-108">None</span></span>

## <a name="methods"></a><span data-ttu-id="7ebd2-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ebd2-109">Methods</span></span>

| <span data-ttu-id="7ebd2-110">Método</span><span class="sxs-lookup"><span data-stu-id="7ebd2-110">Method</span></span>       | <span data-ttu-id="7ebd2-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ebd2-111">Return Type</span></span>  |<span data-ttu-id="7ebd2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ebd2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ebd2-113">Criar Sessão</span><span class="sxs-lookup"><span data-stu-id="7ebd2-113">Create Session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="7ebd2-114">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="7ebd2-114">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="7ebd2-115">Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-115">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="7ebd2-116">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="7ebd2-116">Close Session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="7ebd2-117">None</span><span class="sxs-lookup"><span data-stu-id="7ebd2-117">None</span></span> |<span data-ttu-id="7ebd2-118">Fechar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-118">Close an existing session.</span></span>|
|[<span data-ttu-id="7ebd2-119">Atualizar Sessão</span><span class="sxs-lookup"><span data-stu-id="7ebd2-119">Refresh Session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="7ebd2-120">None</span><span class="sxs-lookup"><span data-stu-id="7ebd2-120">None</span></span> |<span data-ttu-id="7ebd2-121">Atualizar uma sessão existente.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-121">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7ebd2-122">Relações</span><span class="sxs-lookup"><span data-stu-id="7ebd2-122">Relationships</span></span>
| <span data-ttu-id="7ebd2-123">Relação</span><span class="sxs-lookup"><span data-stu-id="7ebd2-123">Relationship</span></span> | <span data-ttu-id="7ebd2-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ebd2-124">Type</span></span>   |<span data-ttu-id="7ebd2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ebd2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ebd2-126">names</span><span class="sxs-lookup"><span data-stu-id="7ebd2-126">names</span></span>|<span data-ttu-id="7ebd2-127">Coleção [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-127">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="7ebd2-p101">Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="7ebd2-130">tables</span><span class="sxs-lookup"><span data-stu-id="7ebd2-130">tables</span></span>|<span data-ttu-id="7ebd2-131">Coleção [WorkbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-131">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="7ebd2-p102">Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="7ebd2-134">worksheets</span><span class="sxs-lookup"><span data-stu-id="7ebd2-134">worksheets</span></span>|<span data-ttu-id="7ebd2-135">Coleção [WorkbookWorksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-135">[WorkbookWorksheet](worksheet.md) collection</span></span>|<span data-ttu-id="7ebd2-p103">Representa uma coleção de planilhas associadas à pasta de trabalho. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="7ebd2-138">Funções</span><span class="sxs-lookup"><span data-stu-id="7ebd2-138">Functions</span></span>

<span data-ttu-id="7ebd2-p104">[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função. O valor `error` de `null` indica a execução bem-sucedida da função.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p104">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="7ebd2-p105">A lista completa de funções com suporte está listada [aqui](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p105">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="7ebd2-144">_Observações importantes:_</span><span class="sxs-lookup"><span data-stu-id="7ebd2-144">_Important notes:_</span></span> 
* <span data-ttu-id="7ebd2-145">O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-145">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="7ebd2-146">O parâmetro index é indexado como 1, diferentemente do índice 0 usado na maioria das APIs.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-146">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="7ebd2-147">Exemplo: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="7ebd2-147">Example: **vlookup**</span></span>

<span data-ttu-id="7ebd2-148">Em uma planilha do Excel, a função `vlookup` utiliza os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="7ebd2-148">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="7ebd2-149">O valor que você deseja pesquisar, também chamado de valor de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-149">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="7ebd2-150">O intervalo em que o valor de pesquisa está localizado.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-150">The range where the lookup value is located.</span></span> <span data-ttu-id="7ebd2-151">Lembre-se de que o valor de pesquisa sempre deve estar na primeira coluna no intervalo para que o PROCV funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-151">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="7ebd2-152">Por exemplo, se o valor de pesquisa estiver na célula C2, o intervalo deve começar com C.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-152">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="7ebd2-153">O número da coluna no intervalo que contém o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-153">The column number in the range that contains the return value.</span></span> <span data-ttu-id="7ebd2-154">Por exemplo, se você especificar B2: D11 como o intervalo, deverá contar B como a primeira coluna, C como a segunda e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-154">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="7ebd2-155">Opcionalmente, você pode especificar TRUE se desejar uma correspondência aproximada ou FALSE se desejar uma correspondência exata do valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-155">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="7ebd2-156">Se você não especificar nada, o valor padrão sempre será TRUE ou uma correspondência aproximada.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-156">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="7ebd2-157">Dentro de uma célula, a função `vlookup` tem esta aparência:</span><span class="sxs-lookup"><span data-stu-id="7ebd2-157">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="7ebd2-158">= PROCV(valor de pesquisa, intervalo que contém o valor de pesquisa, o número da coluna no intervalo que contém o valor de retorno, opcionalmente, TRUE para coincidência aproximada ou FALSE para uma correspondência exata)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-158">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="7ebd2-159">(Confira a documentação para a função do Excel [PROCV](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)).</span><span class="sxs-lookup"><span data-stu-id="7ebd2-159">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="7ebd2-160">O exemplo abaixo mostra como chamar a função `vlookup` e passar esses parâmetros com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-160">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="7ebd2-161">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="7ebd2-161">Request:</span></span> 

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

<span data-ttu-id="7ebd2-162">Resposta:</span><span class="sxs-lookup"><span data-stu-id="7ebd2-162">Response:</span></span>

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

<span data-ttu-id="7ebd2-163">Exemplo: `median`</span><span class="sxs-lookup"><span data-stu-id="7ebd2-163">Example: `median`</span></span>

<span data-ttu-id="7ebd2-164">Em uma planilha do Excel, a função `median` possui uma matriz de um ou mais intervalos de entrada.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-164">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="7ebd2-165">Dentro de uma célula, a função `median` se parece com este exemplo:</span><span class="sxs-lookup"><span data-stu-id="7ebd2-165">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="7ebd2-166">=MED(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-166">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="7ebd2-167">(Confira a documentação para a função [MED](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)).</span><span class="sxs-lookup"><span data-stu-id="7ebd2-167">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="7ebd2-168">O exemplo abaixo mostra como chamar a função `median` e um ou mais intervalos de entrada com a API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-168">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="7ebd2-169">Solicitação:</span><span class="sxs-lookup"><span data-stu-id="7ebd2-169">Request:</span></span> 

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

<span data-ttu-id="7ebd2-170">Resposta:</span><span class="sxs-lookup"><span data-stu-id="7ebd2-170">Response:</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
